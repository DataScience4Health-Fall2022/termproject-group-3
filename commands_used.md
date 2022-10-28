# Commands Used

### Validation runs
General command structure: 
`python validate.py ./mured_single --model MODEL --num-classes 20 --checkpoint ./output/train/CHECKPOINT/model_best.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/MODEL_results.csv`


Metric generation commands

`python validate_extra.py ./mured_single --model vit_base_resnet50d_224 --num-classes 20 --checkpoint ./output/train/20221026-183721-vit_base_resnet50d_224-224/checkpoint-57.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/vit_base_resnet50d_224_results.csv`

`python validate_extra.py ./mured_single --model resnet34 --num-classes 20 --checkpoint ./output/train/20221025-162326-resnet34-224/checkpoint-58.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/resnet34_results.csv`

`python validate_extra.py ./mured_single --model vit_small_patch16_224 --num-classes 20 --checkpoint ./output/train/20221025-170057-vit_small_patch16_224-224/checkpoint-51.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/vit_small_patch16_224_results.csv`

`python validate_extra.py ./mured_single --model vgg16_bn --num-classes 20 --checkpoint ./output/train/20221025-173105-vgg16_bn-224/checkpoint-48.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/vgg16_bn_results.csv`

`python validate_extra.py ./mured_single --model vgg19_bn --num-classes 20 --checkpoint ./output/train/20221026-123451-vgg19_bn-224/checkpoint-61.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/vgg19_bn_results.csv`

`python validate_extra.py ./mured_single --model densenet161 --num-classes 20 --checkpoint ./output/train/20221026-201102-densenet161-224/checkpoint-45.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/densenet161_results.csv`

`python validate_extra.py ./mured_single --model resnet50 --num-classes 20 --checkpoint ./output/train/20221027-133331-resnet50-224/checkpoint-41.pth.tar -b 444 --amp --use-train-size --results-file ./mured_results/resnet50_results.csv`

