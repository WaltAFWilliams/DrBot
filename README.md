# DrBot
Welcome to my diabetic retinopathy classifier. 
I got the original idea to make this deep learning model after reading this paper: https://dl.acm.org/doi/abs/10.1145/3313831.3376718?utm_campaign=The+Batch&utm_medium=email&_hsmi=87523675&_hsenc=p2ANqtz-_B4jFj-cLmuuXwLoX8un3XaSaO0OrwAXpp6Y9Yk9Ubn4cbgJrbAZL9mgbaOt9Qe2dkeCSV&utm_content=87523675&utm_source=hs_email. 

The paper detailed an experiment conducted by researchers at google where they observed how clinics in thailand functioned when using Artificial Intelligence to help with diagnosis of diabetic retinopathy. I urge you to look at the paper as it's very interesting but the gist was they had nurses take pictures of peoples' eyes, then they had a deep learning algorithm process those pictures and determine if it should be sent to an opthalmologist (eye doctor) for further inspection or if it did not contain any levels of DR. That got me wondering if I could potentially build my own Diabetic Retinopathy model and here we are.

The images were downloaded from https://www.kaggle.com/tanlikesmath/diabetic-retinopathy-resized if you would like to play with this dataset on your own.

I tried out several models and ultimately landed on mobilenet as my base model simply due to resource constraints. (When I tried to train EfficientNets or ResNets the process was painfully slow even on my GPU.)
