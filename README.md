# Canvas Mass Avatar Upload by SIS ID

This project is a fork of [this respository](https://github.com/lthh89vt/CanvasMassAvatarUploadSISID).

Which is in turn, a fork of this [this respository](https://github.com/unsupported/canvas/tree/master/api/bulk_assign_avatars/python)

Thank you for your work lthh89vt!

#### Purpose
This Python script will help to mass upload avatar for Canvas users with their SIS ID.
SIS ID is your internal ID when using SIS User Import in Canvas.

This Python script will allow mass uploading of Canvas user avatars. 

#### Requirements
These are the minimum requirements to run this script:
  - Python 2.x
  - Requests module (can be installed via easy-install script)
  - Admin Access Token - [How to generate Access Token](https://guides.instructure.com/m/4214/l/40399-how-do-i-obtain-an-api-access-token-for-an-account) (Need to use admin account)

#### Configuration
These configurations will need to be updated before you can run the script
```sh
domain = '***.instructure.com'
access_token = "ADMIN ACCESS TOKEN"
```

#### CSV File

Please see the sample data.csv for data structure. The columns are:
  - user_id: SIS ID
  - image_filename: Image file name including extension in images/ folder
  - image_filetype: can be jpeg, png or gif

#### Run

```sh
python mass-upload.py
```

#### Support
Let me know if you have any issues and I will attempt to assist. I have run the script successfully from both macOS and Windows. 

I did not write the script, I simply fixed an line that caused the previous project to fail when assigning photos to Canvas users (at least on macOS)

This project is maintained by JKL @ MLC School Sydney
