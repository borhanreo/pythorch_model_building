You need to download data/SIGNS image data


#### IMAGE Crope 64x64

    $ python build_dataset.py --data_dir data/SIGNS --output_dir data/64x64_SIGNS

#### TRAIN
    $ python train.py --data_dir data/64x64_SIGNS --model_dir experiments/base_model
    

#### hyperparameters search . 

    $ python search_hyperparams.py --data_dir data/64x64_SIGNS --parent_dir experiments/learning_rate
    
#### Display the results of the hyperparameters search 

    $ python synthesize_results.py --parent_dir experiments/learning_rate
    
#### Evaluation on the test 

    $ python evaluate.py --data_dir data/64x64_SIGNS --model_dir experiments/base_model
    
    