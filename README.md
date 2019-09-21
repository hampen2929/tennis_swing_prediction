# Tennis swing prediction
This repository is example code for tennis swing prediction.
The artcle in Japanese is here().

## Output movie
![edit2_640](https://user-images.githubusercontent.com/34574033/65372275-b3c29100-dca8-11e9-854f-b4465c12643c.gif)

## Annotation

![image](https://user-images.githubusercontent.com/34574033/65372302-1c117280-dca9-11e9-971e-e6b44faf1b00.png)

## Train and test data

Train

|action|frame count|swing count|
|----|------|---|
|idle|    11384|-|
|forehand|1482|57|
|backhand|1430|55|
|foreslice|1118|43|
|backslice|988|38|

Test

|action|frame count|swing count|
|----|------|---|
|idle|    2850|-|
|forehand|260|10|
|backhand|364|14|
|foreslice|234|9|
|backslice|348|14|

## Plot pose position
![image](https://user-images.githubusercontent.com/34574033/65372315-51b65b80-dca9-11e9-9ecd-7178f2b023c9.png)
forehand

![image](https://user-images.githubusercontent.com/34574033/65372317-57ac3c80-dca9-11e9-9346-c7fc80d0c64b.png)
backhand

![image](https://user-images.githubusercontent.com/34574033/65372319-5a0e9680-dca9-11e9-9424-2c7d16d58013.png)
foreslice

![image](https://user-images.githubusercontent.com/34574033/65372320-5d098700-dca9-11e9-9da7-c4eb482a9196.png)
backslice

## Feature importance
![image](https://user-images.githubusercontent.com/34574033/65372335-87f3db00-dca9-11e9-9c48-b65e0cddfe5b.png)

## Confusion matrix

`Accuracy is 89.32 %`

|             |idle_pred      |forehand_pred  |backhand_pred  |foreslice_pred  |backslice_pred  |
|-------------|---------------|---------------|---------------|----------------|----------------|
|idle_gt      |2684          |14             |40             |13              |99             |
|forehand_gt  |55            |188            |0              |17              |0               |
|backhand_gt  |43             |0              |660            |0               |0               |
|foreslice_gt |87            |12            |0              |135           |0               |
|backslice_gt |52             |0              |1              |0               |295             |
