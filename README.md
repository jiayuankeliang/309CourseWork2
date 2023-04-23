# 309CourseWork2

Hi everyone, this is our project about deep learning!

Cardiff university Msc DSA

group member: Zhang, Guan, Gong, Liang, Brain, Luo, Joe, Sam


# How to execute code
Our data is downloaded directly from kaggle, and you will need to run the following command on your computer：

1.install kaggle plugs.
```
!pip install -q kaggle
```

2.upload your kaggle.json
```
from google.colab import files
files.upload()
```

you can get your kaggle.json in kaggle.com, 'your profile' -> 'Account' -> 'API' -> 'Create New Token'

3.run these code, copy kaggle.json to local and change the file permission
```
! mkdir ~/.kaggle
! cp kaggle.json ~/.kaggle/
! chmod 600  ~/.kaggle/kaggle.json
```

4.download data
```
!kaggle datasets download meowmeowmeowmeowmeow/gtsrb-german-traffic-sign
```

5.unzip the data
```
import zipfile

filename = '/content/gtsrb-german-traffic-sign.zip'

with zipfile.ZipFile(filename, 'r') as zip_ref:
  zip_ref.extractall('.')
```

Now that the data is ready, you can run the next part of the code, you don't need to run the above separately, it's already included in our code, you just need to upload your kaggle.json