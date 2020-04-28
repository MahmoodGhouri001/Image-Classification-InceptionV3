

## Transfer learning using Tensorflow on Inception-V3 model



#### Transfer learning


We will train the Inception-V3 model with our own set of images present in process_files folder.

The folder documents contains the images of 3 types of documents:
  1. Form1
  2. Form2
  3. Form2

Execute the following command in your terminal to retrain the model

`
$ python retrain.py --output_graph=process_files/retrained_graph.pb --output_labels=process_files/retrained_labels.txt --image_dir=process_files/train_input_data
`
>it will start training and complete around 4000 steps


Execute the following command in your terminal to verify the results
`$ python label.py --image test11/11.jpg`

```

After execution above command it will generate result folder at current working directory and contains classes and keep the classified images in it.


