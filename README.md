# live_templates_getx_android_studio
This is a repo aiming to simplify and accelerate development time of Flutter apps based on GetX package.
In this repo you can find handy live templates to shape up your UI faster.

# How to install live templates
In order to install them you need to download xml file in the root of this repo and place it inside templates folder of Android Studio.
Depending on OS you are using the path to templates folder may differ. Here are paths:
Windows:<your_user_home_directory>\.AndroidStudio<version_number>\config\templates




Linux: ~/.AndroidStudio<version>/config/templates



MacOS: ~/Library/Preferences/AndroidStudio<version>/templates
# Usage

# gxcon - to create GetxController

class $NAME$PageController extends GetxController {
    $END$
}

# gxvwb - to create GetView with GetBuilder and GetxController

class $NAME$Page extends GetView<$NAME$PageController> {
  @override
  Widget build(BuildContext context) {
    return GetBuilder<$NAME$PageController>(
     builder: (value) => Scaffold(
        body: Container($END$),
      ),
    );
  }
}

class $NAME$PageController extends GetxController {}


# gxv - to create GetView with GetxController

class $PAGE_NAME$Page
    extends GetView<$PAGE_NAME$PageController> {
 @override
  Widget build(BuildContext context) {
    return Container($END$);
  }
}
class $PAGE_NAME$PageController extends GetxController {}


# gxbind - to create Bindings

class $BUNDING_NAME$ implements Bindings {
  @override
  void dependencies() {
    // TODO: implement dependencies
  }
}


# gxlzput - to put GetxController to Binding lazyly

Get.lazyPut<$CONTROLLER_NAME$>(
    () => $CONTROLLER_NAME$(),
    fenix: true,
);

# Enjoy it!
