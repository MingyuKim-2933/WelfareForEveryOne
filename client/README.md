# 모두의 복지
## App Development
- 모두의 복지 어플리케이션
- Android Studio 2020.03.01 patch2
- program language : Java
- MapActivity : Google Map API 활용
- http: Volley Module

## How to execute
```
sync project with gradle files
build project
run app
```

## 프로젝트 구조
```
├── AndroidManifest.xml
├── ic_launcher_new-playstore.png
├── java
│   └── com
│       └── product
│           └── welfareapp
│               ├── AppHelper.java
│               ├── ChatActivity.java
│               ├── ChatModel.java
│               ├── ChatRVAdapter.java
│               ├── DetailActivity.java
│               ├── IntroActivity.java
│               ├── ListActivity.java
│               ├── LoginActivity.java
│               ├── MainActivity.java
│               ├── MainCategoryCard.java
│               ├── MainRVAdapter.java
│               ├── MainViewAllActivity.java
│               ├── MapActivity.java
│               ├── MyFirebaseMessagingService.java
│               ├── MyProfileActivity.java
│               ├── MyProfileListActivity.java
│               ├── ProfileActivity.java
│               ├── PushActivity.java
│               ├── PushNotificationComponent.java
│               ├── PushViewAdapter.java
│               ├── RegisterActivity.java
│               ├── URLs.java
│               ├── User.java
│               ├── UserLoginInfo.java
│               ├── VolleySingleton.java
│               ├── WebViewActivity.java
│               ├── WelfareInfoComponent.java
│               └── WelfareViewAdapter.java
├── res
│   ├── drawable
│   │   ├── bot_msg_box_container.xml
│   │   ├── bottom_menu_ico_1.png
│   │   ├── bottom_menu_ico_2.png
│   │   ├── bottom_menu_ico_3.png
│   │   ├── bottom_menu_ico_4.png
│   │   ├── btn_container_map.xml
│   │   ├── btn_design.xml
│   │   ├── btn_design_login.xml
│   │   ├── btn_design_map.xml
│   │   ├── btn_edit_profile.xml
│   │   ├── btn_view_more.xml
│   │   ├── card_component_container.xml
│   │   ├── chatbot_icon_temp.xml
│   │   ├── day_notify_container.xml
│   │   ├── detail_picture.xml
│   │   ├── et_design_login.xml
│   │   ├── et_design_register.xml
│   │   ├── ic_arrow_back.xml
│   │   ├── ic_back.xml
│   │   ├── ic_btn_back_white.xml
│   │   ├── ic_category_btn.xml
│   │   ├── ic_category_btn2.xml
│   │   ├── ic_launcher_background.xml
│   │   ├── ic_launcher_foreground.xml
│   │   ├── ic_launcher_new_background.xml
│   │   ├── ic_logout.xml
│   │   ├── ic_logout2.xml
│   │   ├── ic_push_notification.xml
│   │   ├── ic_push_notification2.xml
│   │   ├── ic_search.xml
│   │   ├── ic_speach_btn.xml
│   │   ├── ic_user_profile.jpg
│   │   ├── img_category_00.jpg
│   │   ├── img_category_01.jpg
│   │   ├── img_category_02.jpg
│   │   ├── img_category_03.jpg
│   │   ├── img_category_04.jpg
│   │   ├── img_category_05.jpg
│   │   ├── img_category_06.jpg
│   │   ├── img_category_07.jpg
│   │   ├── img_category_08.jpg
│   │   ├── img_category_09.jpg
│   │   ├── img_category_10.jpg
│   │   ├── img_category_11.jpg
│   │   ├── img_category_12.jpg
│   │   ├── img_category_13.jpg
│   │   ├── img_category_14.jpg
│   │   ├── img_category_15.jpg
│   │   ├── img_icon_00.jpg
│   │   ├── img_icon_01.jpg
│   │   ├── img_icon_02.jpg
│   │   ├── img_icon_03.jpg
│   │   ├── img_icon_04.jpg
│   │   ├── img_icon_05.jpg
│   │   ├── img_icon_06.jpg
│   │   ├── img_icon_07.jpg
│   │   ├── img_icon_08.jpg
│   │   ├── img_icon_09.jpg
│   │   ├── img_icon_10.jpg
│   │   ├── img_icon_11.jpg
│   │   ├── img_icon_12.jpg
│   │   ├── img_icon_13.jpg
│   │   ├── img_icon_14.jpg
│   │   ├── img_icon_15.jpg
│   │   ├── img_main_logo.png
│   │   ├── intro_background.png
│   │   ├── intro_background_fit.png
│   │   ├── map_btn_design.xml
│   │   ├── map_icon_hospital.xml
│   │   ├── map_icon_local_hospital.xml
│   │   ├── map_icon_obstacle.xml
│   │   ├── map_icon_office.xml
│   │   ├── map_icon_police.xml
│   │   ├── menu_chat.xml
│   │   ├── menu_home.xml
│   │   ├── menu_map.xml
│   │   ├── menu_pf.xml
│   │   ├── menu_push.xml
│   │   ├── menu_selector_color.xml
│   │   ├── photo_button.png
│   │   ├── profile_default.png
│   │   ├── profile_edit_icon.xml
│   │   ├── push_list_container.xml
│   │   ├── recommend_list_container.xml
│   │   ├── shadow.xml
│   │   ├── toggle_button_off.xml
│   │   ├── toggle_button_off2.png
│   │   ├── toggle_button_on.xml
│   │   ├── toggle_button_on2.xml
│   │   ├── toggle_button_selector.xml
│   │   ├── tv_design_chat.xml
│   │   ├── tv_main_info_container.xml
│   │   └── user_msg_box_container.xml
│   ├── drawable-v24
│   │   └── ic_launcher_foreground.xml
│   ├── font
│   │   ├── font.xml
│   │   ├── noto_sans_kr_black.otf
│   │   ├── noto_sans_kr_bold.otf
│   │   ├── noto_sans_kr_light.otf
│   │   ├── noto_sans_kr_medium.otf
│   │   ├── noto_sans_kr_regular.otf
│   │   └── noto_sans_kr_thin.otf
│   ├── layout
│   │   ├── activity_chat.xml
│   │   ├── activity_detail.xml
│   │   ├── activity_intro.xml
│   │   ├── activity_list.xml
│   │   ├── activity_login.xml
│   │   ├── activity_main.xml
│   │   ├── activity_main_view_all.xml
│   │   ├── activity_map.xml
│   │   ├── activity_my_profile.xml
│   │   ├── activity_my_profile_list.xml
│   │   ├── activity_profile.xml
│   │   ├── activity_push.xml
│   │   ├── activity_register.xml
│   │   ├── activity_web_view.xml
│   │   ├── bot_info_toolbox.xml
│   │   ├── bot_msg_toolbox.xml
│   │   ├── bot_msg_toolbox2.xml
│   │   ├── card_component.xml
│   │   ├── card_component_notification.xml
│   │   ├── category_select_component.xml
│   │   ├── toolbar_chatbot.xml
│   │   ├── toolbar_info_detail.xml
│   │   ├── toolbar_main.xml
│   │   ├── toolbar_main_info.xml
│   │   ├── toolbar_main_list.xml
│   │   ├── toolbar_profile_edit.xml
│   │   ├── toolbar_profile_list.xml
│   │   ├── toolbar_push.xml
│   │   ├── toolbar_register.xml
│   │   └── user_msg_toolbox.xml
│   ├── menu
│   │   └── bottom_nav.xml
│   ├── mipmap-anydpi-v26
│   │   ├── ic_launcher.xml
│   │   ├── ic_launcher_new.xml
│   │   ├── ic_launcher_new_round.xml
│   │   └── ic_launcher_round.xml
│   ├── mipmap-hdpi
│   │   ├── ic_launcher.webp
│   │   ├── ic_launcher_new.png
│   │   ├── ic_launcher_new_foreground.png
│   │   ├── ic_launcher_new_round.png
│   │   └── ic_launcher_round.webp
│   ├── mipmap-mdpi
│   │   ├── ic_launcher.webp
│   │   ├── ic_launcher_new.png
│   │   ├── ic_launcher_new_foreground.png
│   │   ├── ic_launcher_new_round.png
│   │   └── ic_launcher_round.webp
│   ├── mipmap-xhdpi
│   │   ├── ic_launcher.webp
│   │   ├── ic_launcher_new.png
│   │   ├── ic_launcher_new_foreground.png
│   │   ├── ic_launcher_new_round.png
│   │   └── ic_launcher_round.webp
│   ├── mipmap-xxhdpi
│   │   ├── ic_launcher.webp
│   │   ├── ic_launcher_new.png
│   │   ├── ic_launcher_new_foreground.png
│   │   ├── ic_launcher_new_round.png
│   │   └── ic_launcher_round.webp
│   ├── mipmap-xxxhdpi
│   │   ├── ic_launcher.webp
│   │   ├── ic_launcher_new.png
│   │   ├── ic_launcher_new_foreground.png
│   │   ├── ic_launcher_new_round.png
│   │   └── ic_launcher_round.webp
│   ├── raw
│   │   ├── firstanimation.json
│   │   └── happychatbot.json
│   ├── values
│   │   ├── colors.xml
│   │   ├── strings.xml
│   │   └── themes.xml
│   ├── values-night
│   │   └── themes.xml
│   └── xml
│       └── network_security_config.xml
└── welfareapp_structure.txt
20 directories, 199 files
```
* 본 프로젝트는 Google의 GCP Credit 지원을 받고 있습니다. (Google supported this work by providing Google Cloud credit)