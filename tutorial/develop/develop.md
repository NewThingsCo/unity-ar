# How to develop your first AR app

## Register to Vuforia

1. Browse to [Vuforia register page](https://developer.vuforia.com/vui/auth/register)
2. Register
3. Get development license key

    ![Vuforia development key screenshot](screenshots/1_dev-license-key.png)
    ![Vuforia create development key screenshot](screenshots/2_create-dev-license-key.png)

## Create image target

About image targets on [Vuforia developer library](https://library.vuforia.com/articles/Training/Image-Target-Guide)

1. Create database for image targets

    ![Vuforia target database screenshot](screenshots/3_target-database.png)
    ![Vuforia create target database screenshot](screenshots/4_create-database.png)

2. Add image target to database

    In this tutorial we will use simple 2D image as a target. Set image width to 1 for convenience.

    ![Vuforia add image target screenshot](screenshots/5_add-target.png)
    ![Vuforia upload image target screenshot](screenshots/6_upload-target.png)

## Import image target package to Unity

1. Download image target database

    ![Download image target database screenshot](screenshots/7_download-database.png)
    ![Download image target database for unity screenshot](screenshots/8_download-database-unity.png)

2. Create new Unity project

    ![Create new Unity project screenshot](screenshots/9_create-unity-project.png)

3. Import image target package

    Assets > Import Package > Custom Package
    ![Import image package to Unity screenshot](screenshots/10_import-package.png)
    ![Import image package to Unity screenshot](screenshots/11_import-package-2.png)

## Start developing

1. Create new scene

    File > New Scene
    ![Create new scene screenshot](screenshots/12_create-new-scene.png)

2. Activate Vuforia

    Edit > Project Settings > Player
    ![Activate Vuforia screenshot](screenshots/6_activate-vuforia.png)

3. Add AR camera to scene

    GameObject > Vuforia > AR Camera
    ![Add AR camera screenshot](screenshots/13_add-ar-camera.png)

4. Add license to Vuforia config

    Select AR camera, copy Vuforia license from [License Manager](https://developer.vuforia.com/targetmanager/licenseManager) and paste it to Vuforia config in Unity.

    ![Open Vuforia config screenshot](screenshots/14_open-vuforia-config.png)
    ![Copy Vuforia license screenshot](screenshots/15_copy-license.png)
    ![Paste Vuforia license screenshot](screenshots/16_add-license.png)

5. Add image target to scene

    ![Add image target to scene screenshot](screenshots/17_add-image-target.png)

6. Attach object to image target

    To show something when your image target is detected, you have to attach some object to image target. Simple cube is a good starting point. You can configure size and the position of the cube relative to the image target from the right side panel.

    ![Attach object to image target screenshot](screenshots/18_add-cube.png)

7. Attach spin script to cube object

    ![Attach spin script screenshot](screenshots/20_add-script.png)

    Copy code below to script file

    ```c#
    using UnityEngine;
    using System.Collections;

    public class Spin : MonoBehaviour
    {
        public float speed = 50f;

        void Update ()
        {
            transform.Rotate(Vector3.up, speed * Time.deltaTime);
        }
    }
    ```

8. Save your scene

    ![Save scene screenshot](screenshots/19_save-scene.png)

## [Build and deploy!](../build/build.md)

Now you should have App that shows spinning cube floating when your image target is detected!
