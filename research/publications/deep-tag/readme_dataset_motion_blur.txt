# DeepTag dataset - motion blur part

## File structure
Folder names are in the format of `imgs_0ABC`, where
- "A" is the marker family, and 0~6 represents AprilTag, ArUco, ARToolKitPlus, TopoTag, AprilTag-XO, AprilTag-XA and RuneTag(+) respectively.
- "B" is the view angle, and 0~9 represents 0, 10, 20, 30, 40, 50, 60, 65, 70, and 75 deg respectively.
- "C" is the view distance, and 0~9 represents 10, 20, 30, 40, 50, 60, 70, 80, 90, and 100 cm respectively.

Each folder contains images of the same marker, view distance, and view angle, but with different levels of motion blur.
Image file names are in the format of `DDDD_EEEEEE`, where
- "DDDD" represents motion blur level, and the kernel size `k = DDDD * 2 + 1`, e.g, "0005" represents `k = 11`.
- For each motion blur level, "EEEEEE" represents 10 evenly sampled directions for motion blur, i.e, 0, 10, 20, 30, 40, 50, 60, 70, 80, and 90 deg.


## Terms of use
The dataset is provided for research purposes only. Any commercial use is prohibited. When using the dataset in your research work, please cite the following paper:

	"DeepTag: A General Framework for Fiducial Marker Design and Detection." 
	Zhuming Zhang, Yongtao Hu, Guoxing Yu, and Jingwen Dai  
	arXiv:2105.13731 (2021).

	@article{zhang2021deeptag,
	  title={{DeepTag: A General Framework for Fiducial Marker Design and Detection}},
	  author={Zhang, Zhuming and Hu, Yongtao and Yu, Guoxing and Dai, Jingwen},
	  year={2021},
	  eprint={2105.13731},
	  archivePrefix={arXiv},
	  primaryClass={cs.CV}
	}
