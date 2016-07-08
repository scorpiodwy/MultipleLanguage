This app is to test multiple language in Android.

java:
MainActivity is the main activity, with implementation of language selection function.
Main2Activity is the second activity, not being modified.
Show is the third activity, not being modified.

res:
menu/menu_main.xml, there are 5 items in SETTINGS.
values/strings.xml, there are 4 strings.xml files, which are in en, es, fr, and zh. Right click any of them and select "Open Translations Editor", you can see the key-values pairs clearly.
In the default strings.xml (without any language code), there is an array letting user select language.
layout/content_main.xml, there is a button with text "Click Me". Click this button will redirect user to layout/activity_main2.xml.
In layout/activity_main2.xml, there is a textview, which will be shown Hello in different languages.
layout/activity_show.xml, there is a spinner, which refers to the array in strings.xml.

Main function:
1. Click the SETTINGS in right-top corner, and select change language.
2. Select one language you want, and click OK.
3. All texts will be changed automatically referring to the language you just selected.
4. Click button "Click Me", the Hello is also changed to different language.
This app shows once we modify the language using Configuration.locale, everything will be changed automatically, and it is unnecessary to use broadcaster, value-passing between activities, and others.