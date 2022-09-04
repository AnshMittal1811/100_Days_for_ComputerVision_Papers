# 365 Days for Computer Vision Research

* **Day 1 (01/01/2022)**: [Deep Vehicle Detection in Satellite Videos](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/001%20Deep%20Vehicle%20Detection%20in%20Satellite%20Video.pdf)

**Abstract—** This work presents a deep learning approach for vehicle detection in satellite video. Vehicle detection is perhaps impossible in single EO satellite images due to the tininess of vehicles (4-10 pixel) and their similarity to the background. Instead, we consider satellite video which overcomes the lack of spatial information by temporal consistency of vehicle movement. A new spatiotemporal model of a compact 3 × 3 convolutional, neural network is proposed which neglects pooling layers and uses leaky ReLUs. Then we use a reformulation of the output heatmap including Non-Maximum-Suppression (NMS) for the final segmentation. Empirical results on two new annotated satellite videos reconfirm the applicability of this approach for vehicle detection. They more importantly indicate that pretraining on WAMI data and then fine-tuning on few annotated video frames for a new video is sufficient. In our experiment only five annotated images yield a 𝐹1 score of 0.81 on a new video showing more complex traffic patterns than the Las Vegas video. Our best result on Las Vegas is a 𝐹1 score of 0.87 which makes the proposed approach a leading method for this benchmark.

* **Day 2 (01/02/2022)**: [Pyramidial Attention for Saliency Detection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/002%20Pyramidal%20Attention%20for%20Saliency%20Detection.pdf)

**Abstract—** Salient object detection (SOD) extracts meaningful contents from an input image. RGB-based SOD methods lack the complementary depth clues; hence, providing limited performance for complex scenarios. Similarly, RGB-D models process RGB and depth inputs, but the depth data availability during testing may hinder the model’s practical applicability. This paper exploits only RGB images, estimates depth from RGB, and leverages the intermediate depth features. We employ a pyramidal attention structure to extract multi-level convolutional-transformer features to process initial stage representations and further enhance the subsequent ones. At each stage, the backbone transformer model produces global receptive fields and computing in parallel to attain fine-grained global predictions refined by our residual convolutional attention decoder for optimal saliency prediction. We report significantly improved performance against 21 and 40 state-ofthe-art SOD methods on eight RGB and RGB-D datasets, respectively. Consequently, we present a new SOD perspective of generating RGB-D SOD without acquiring depth data during training and testing and assist RGB methods with depth clues for improved performance. The code and trained models are available at https://github.com/tanveer-hussain/EfficientSOD2

* **Day 3 (01/03/2022)**: [Human Identity-Preserved Motion Retargeting in Video Synthesis by Feature Diseentanglement](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/003%20Human%20Identity%20Preserved%20Motion%20Retargeting%20in%20Video%20Synthesis%20by%20Feature%20Disentanglement.pdf)

**Abstract—** Most motion retargeting methods in human action video synthesis decompose the input video to motion (dynamic information) and shape (static information). However, we observe if the dynamic information is directly transferred to another subject, it will result in unnatural synthesised motion. This phenomenon is mainly caused by neglecting subject-dependent information in motion. To solve the problem, we propose a novel motion retargeting method which can combine both subject-independent (common motion content) information from a source video and subject-dependent (individualized identity motion) information from a target video. So it can synthesize videos with a much natural appearance along with identity-preserved motion (Figure 1). In the proposed method two encoders are employed to extract identity and motion content representations respectively. We employ the adaptive instance normalization (AdaIN) layer in the generator and the instance normalization (IN) layer in the motion content encoder to synthesize the new motion. Besides, we also collected a dataset, named𝐶ℎ𝑢𝑎𝑛𝑔101, with 101 subjects in total. Each subject performs identical dancing movement, and so it is convenient for feature disentanglement among motion and identity of each subject. Furthermore, an efficient quantitative metric for identify information is designed by gait recognition. The experiments show the proposed method cansynthesize videos more naturally when the subject’s identity is preserved.


* **Day 4 (01/04/2022)**: [Implicit Sample Extension for Unsupervised Person ReIdentification](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/004%20Implicit%20Sample%20Extension%20for%20Unsupervised%20Person%20ReIdentification.pdf)

**Abstract—** Most existing unsupervised person re-identification (ReID) methods use clustering to generate pseudo labels for model training. Unfortunately, clustering sometimes mixes different true identities together or splits the same identity into two or more sub clusters. Training on these noisy clusters substantially hampers the Re-ID accuracy. Due to the limited samples in each identity, we suppose there may lack some underlying information to well reveal the accurate clusters. To discover these information, we propose an Implicit Sample Extension (ISE) method to generate what we call support samples around the cluster boundaries. Specifically, we generate support samples from actual samples and their neighbouring clusters in the embedding space through a progressive linear interpolation (PLI) strategy. PLI controls the generation with two critical factors, i.e., 1) the direction from the actual sample towards its K-nearest clusters and 2) the degree for mixing up the context information from the K-nearest clusters. Meanwhile, given the support samples, ISE further uses a label-preserving loss to pull them towards their corresponding actual samples, so as to compact each cluster. Consequently, ISE reduces the “sub and mixed” clustering errors, thus improving the Re-ID performance. Extensive experiments demonstrate that the proposed method is effective and achieves state-of-the-art performance for unsupervised person Re-ID. Code is available at: https://github.com/PaddlePaddle/PaddleClas.

* **Day 5 (01/05/2022)**: [GIFS: Neural Implicit Function for General Shape Representation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/005%20GIFS-%20Neural%20Implicit%20Function%20for%20General%20Shape%20Representation.pdf)

**Abstract—** Recent development of neural implicit function has shown tremendous success on high-quality 3D shape reconstruction. However, most works divide the space into inside and outside of the shape, which limits their representing power to single-layer and watertight shapes. This limitation leads to tedious data processing (converting nonwatertight raw data to watertight) as well as the incapability of representing general object shapes in the real world. In this work, we propose a novel method to represent general shapes including non-watertight shapes and shapes with multi-layer surfaces. We introduce General Implicit Function for 3D Shape (GIFS), which models the relationships between every two points instead of the relationships between points and surfaces. Instead of dividing 3D space into predefined inside-outside regions, GIFS encodes whether two points are separated by any surface. Experiments on ShapeNet show that GIFS outperforms previous state-of-the-art methods in terms of reconstruction quality, rendering efficiency, and visual fidelity. Project page is available at https://jianglongye.com/gifs.

* **Day 6 (01/06/2022)**: [XCiT: Cross Covariance Image Transformers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/006%20XCiT%20Cross%20Covariance%20Image%20Transformers.pdf)

**Abstract—** Following tremendous success in natural language processing, transformers have recently shown much promise for computer vision. The self-attention operation underlying transformers yields global interactions between all tokens, i.e. words or image patches, and enables flexible modelling of image data beyond the local interactions of convolutions. This flexibility, however, comes with a quadratic complexity in time and memory, hindering application to long sequences and highresolution images. We propose a “transposed” version of self-attention that operates across feature channels rather than tokens, where the interactions are based on the cross-covariance matrix between keys and queries. The resulting cross-covariance attention (XCA) has linear complexity in the number of tokens, and allows efficient processing of high-resolution images. Our cross-covariance image transformer (XCiT) – built upon XCA – combines the accuracy of conventional transformers with the scalability of convolutional architectures. We validate the effectiveness and generality of XCiT by reporting excellent results on multiple vision benchmarks, including (self-supervised) image classification on ImageNet-1k, object detection and instance segmentation on COCO, and semantic segmentation on ADE20k

* **Day 7 (01/07/2022)**: [Partial Membership Latent Dirichlet Allocation for Image Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/007%20Partial%20Membership%20Latent%20Dirichlet%20Allocation%20for%20Image%20Segmentation.pdf)

**Abstract—** —Topic models (e.g., pLSA, LDA, SLDA) have been widely used for segmenting imagery. These models are confined to crisp segmentation. Yet, there are many images in which some regions cannot be assigned a crisp label (e.g., transition regions between a foggy sky and the ground or between sand and water at a beach). In these cases, a visual word is best represented with partial memberships across multiple topics. To address this, we present a partial membership latent Dirichlet allocation (PM-LDA) model and associated parameter estimation algorithms. Experimental results on two natural image datasets and one SONAR image dataset show that PM-LDA can produce both crisp and soft semantic image segmentations; a capability existing methods do not have.

* **Day 8 (01/08/2022)**: [Photorealistic Monocular 3D Reconstruction of Humans Wearing Clothing](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/008%20Photorealistic%20Monocular%203D%20Reconstruction%20of%20Humans%20Wearing%20Clothing.pdf)

**Abstract—** We present PHORHUM, a novel, end-to-end trainable, deep neural network methodology for photorealistic 3D human reconstruction given just a monocular RGB image. Our pixel-aligned method estimates detailed 3D geometry and, for the first time, the unshaded surface color together with the scene illumination. Observing that 3D supervision alone is not sufficient for high fidelity color reconstruction, we introduce patch-based rendering losses that enable reliable color reconstruction on visible parts of the human, and detailed and plausible color estimation for the non-visible parts. Moreover, our method specifically addresses methodological and practical limitations of prior work in terms of representing geometry, albedo, and illumination effects, in an end-to-end model where factors can be effectively disentangled. In extensive experiments, we demonstrate the versatility and robustness of our approach. Our state-of-the-art results validate the method qualitatively and for different metrics, for both geometric and color reconstruction.

* **Day 9 (01/09/2022)**: [Dress Code: High-Resolution Multi-category Virtual Try-On](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/009%20DressCode%20High-Resolution%20Multi-Category%20Virtual%20Try-On.pdf)

**Abstract—** Image-based virtual try-on strives to transfer the appearance of a clothing item onto the image of a target person. Prior work focuses mainly on upper-body clothes (e.g. t-shirts, shirts, and tops) and neglects full-body or lower-body items. This shortcoming arises from amain factor: current publicly available datasets for image-based virtual try-on do not account for this variety, thus limiting progress in the field. To address this deficiency, we introduce Dress Code, which contains images of multi-category clothes. Dress Code is more than 3× larger than publicly available datasets for image-based virtual try-on and features high-resolution paired images (1024 × 768) with front-view, full-body reference models. To generate HD try-on images with high visual quality and rich in details, we propose to learn fine-grained discriminating features. Specifically, we leverage a semantic-aware discriminator that makes predictions at pixel-level instead of image- or patch-level. Extensive experimental evaluation demonstrates that the proposed approach surpasses the baselines and state-of-the-art competitors in terms of visual quality and quantitative results. The Dress Code dataset is publicly available at https://github.com/aimagelab/dress-code.

* **Day 10 (01/10/2022)**: [Pyramid Grafting Network for One-Stage High Resolution Saliency Detection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/010%20Pyramid%20Grafting%20Network%20for%20OneStage%20HighResolution%20Saliency%20Detection.pdf)

**Abstract—** Recent salient object detection (SOD) methods basedon deep neural network have achieved remarkable performance. However, most of existing SOD models designed for low-resolution input perform poorly on high-resolution images due to the contradiction between the sampling depth and the receptive field size. Aiming at resolving this contradiction, we propose a novel one-stage framework called Pyramid Grafting Network (PGNet), using transformer and CNN backbone to extract features from different resolution images independently and then graft the features from transformer branch to CNN branch. An attention-based Cross-Model Grafting Module (CMGM) is proposed to enable CNN branch to combine broken detailed information more holistically, guided by different source feature during decoding process. Moreover, we design an Attention Guided Loss (AGL) to explicitly supervise the attention matrix generated by CMGM to help the network better interact with the attention from different models. We contribute a new Ultra-High-Resolution Saliency Detection dataset UHRSD, containing 5,920 images at 4K-8K resolutions. To our knowledge, it is the largest dataset in both quantity and resolution for high-resolution SOD task, which can be used for training and testing in future research. Sufficient experiments on UHRSD and widely-used SOD datasets demonstrate that our method achieves superior performance compared to the state-of-the-art methods.

* **Day 11 (01/11/2022)**: [Searching Intrinsic Dimensions of Vision Transformers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/011%20Searching%20Intrinsic%20Dimensions%20of%20Vision%20Transformers.pdf)

**Abstract—** It has been shown by many researchers that transformers perform as well as convolutional neural networks in many computer vision tasks. Meanwhile, the large computational costs of its attention module hinder further studies and applications on edge devices. Some pruning methods have been developed to construct efficient vision transformers, but most of them have considered image classification tasks only. Inspired by these results, we propose SiDT, a method for pruning vision transformer backbones on more complicated vision tasks like object detection, based on the search of transformer dimensions. Experiments on CIFAR-100 and COCO datasets show that the backbones with 20\% or 40\% dimensions/parameters pruned can have similar or even better performance than the unpruned models. Moreover, we have also provided the complexity analysis and comparisons with the previous pruning methods.

* **Day 12 (01/12/2022)**: [OSSO: Obtaining Skeletal Shape from Outside](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/012%20OSSO%20Obtaining%20Skeletal%20Shape%20from%20Outside.pdf) 

**Abstract—** We address the problem of inferring the anatomic skeleton of a person, in an arbitrary pose, from the 3D surface of the body; i.e. we predict the inside (bones) from the outside (skin). This has many applications in medicine and biomechanics. Existing state-of-the-art biomechanical skeletons are detailed but do not easily generalize to new subjects. Additionally, computer vision and graphics methods that predict skeletons are typically heuristic, not learned from data, do not leverage the full 3D body surface, and are not validated against ground truth. To our knowledge, our system, called OSSO (Obtaining Skeletal Shape from Outside), is the first to learn the mapping from the 3D body surface to the internal skeleton from real data. We do so using 1000 male and 1000 female dual-energy X-ray absorptiometry (DXA) scans. To these, we fit a parametric 3D body shape model (STAR) to capture the body surface and a novel part-based 3D skeleton model to capture the bones. This provides inside/outside training pairs. We model the statistical variation of full skeletons using PCA in a pose-normalized space. We then train a regressor from body shape parameters to skeleton shape parameters and refine the skeleton to satisfy constraints on physical plausibility. Given an arbitrary 3D body shape and pose, OSSO predicts a realistic skeleton inside. In contrast to previous work, we evaluate the accuracy of the skeleton shape quantitatively on held-out DXA scans, outperforming the state-of-the-art. We also show 3D skeleton prediction from varied and challenging 3D bodies. The code to infer a skeleton from a body shape is available for research at this https URL, and the dataset of paired outer surface (skin) and skeleton (bone) meshes is available as a Biobank Returned Dataset. This research has been conducted using the UK Biobank Resource.

* **Day 13 (01/13/2022)**: [SelfD: Self-Learning Large-Scale Driving Policies From the Web](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/013%20SelfD%20Self-Learning%20Large-Scale%20Driving%20Policies%20From%20the%20Web.pdf)

**Abstract—** Effectively utilizing the vast amounts of ego-centric navigation data that is freely available on the internet can advance generalized intelligent systems, i.e., to robustly scale across perspectives, platforms, environmental conditions, scenarios, and geographical locations. However, it is difficult to directly leverage such large amounts of unlabeled and highly diverse data for complex 3D reasoning and planning tasks. Consequently, researchers have primarily focused on its use for various auxiliary pixel- and image-level computer vision tasks that do not consider an ultimate navigational objective. In this work, we introduce SelfD, a framework for learning scalable driving by utilizing large amounts of online monocular images. Our key idea is to leverage iterative semi-supervised training when learning imitative agents from unlabeled data. To handle unconstrained viewpoints, scenes, and camera parameters, we train an image-based model that directly learns to plan in the Bird's Eye View (BEV) space. Next, we use unlabeled data to augment the decision-making knowledge and robustness of an initially trained model via self-training. In particular, we propose a pseudo-labeling step which enables making full use of highly diverse demonstration data through "hypothetical" planning-based data augmentation. We employ a large dataset of publicly available YouTube videos to train SelfD and comprehensively analyze its generalization benefits across challenging navigation scenarios. Without requiring any additional data collection or annotation efforts, SelfD demonstrates consistent improvements (by up to 24%) in driving performance evaluation on nuScenes, Argoverse, Waymo, and CARLA.

* **Day 14 (01/14/2022)**: [Analysis of the Possibilities of Tire-Defect Inspection based on Unsupervised Learning and Deep Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/014%20Analysis%20of%20the%20Possibilities%20of%20Tire-Defect%20Inspection%20Based%20on%20Unsupervised%20Learning%20and%20Deep%20Learning.pdf)

**Abstract—** At present, inspection systems process visual data captured by cameras, with deep learning approaches applied to detect defects. Defect detection results usually have an accuracy higher than 94%. Real-life applications, however, are not very common. In this paper, we describe the development of a tire inspection system for the tire industry. We provide methods for processing tire sidewall data obtained from a camera and a laser sensor. The captured data comprise visual and geometric data characterizing the tire surface, providing a real representation of the captured tire sidewall. We use an unfolding process, that is, a polar transform, to further process the camera-obtained data. The principles and automation of the designed polar transform, based on polynomial regression (i.e., supervised learning), are presented. Based on the data from the laser sensor, the detection of abnormalities is performed using an unsupervised clustering method, followed by the classification of defects using the VGG-16 neural network. The inspection system aims to detect trained and untrained abnormalities, namely defects, as opposed to using only supervised learning methods. View Full-Text

* **Day 15 (01/15/2022)**: [Self-Supervised Camera Self-Calibration from Video](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/015%20Self-Supervised%20Camera%20Self-Calibration%20from%20Video.pdf)

**Abstract—** Camera calibration is integral to robotics and computer vision algorithms that seek to infer geometric properties of the scene from visual input streams. In practice, calibration is a laborious procedure requiring specialized data collection and careful tuning. This process must be repeated whenever the parameters of the camera change, which can be a frequent occurrence for mobile robots and autonomous vehicles. In contrast, self-supervised depth and ego-motion estimation approaches can bypass explicit calibration by inferring per-frame projection models that optimize a view synthesis objective. In this paper, we extend this approach to explicitly calibrate a wide range of cameras from raw videos in the wild. We propose a learning algorithm to regress per-sequence calibration parameters using an efficient family of general camera models. Our procedure achieves self-calibration results with sub-pixel reprojection error, outperforming other learning-based methods. We validate our approach on a wide variety of camera geometries, including perspective, fisheye, and catadioptric. Finally, we show that our approach leads to improvements in the downstream task of depth estimation, achieving state-of-the-art results on the EuRoC dataset with greater computational efficiency than contemporary methods.

* **Day 16 (01/16/2022)**: [BlobGAN: Spatially Disentangled Scene Representations](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/016%20BlobGAN.pdf)

**Abstract—** We propose an unsupervised, mid-level representation for a generative model of scenes. The representation is mid-level in that it is neither per-pixel nor per-image; rather, scenes are modeled as a collection of spatial, depth-ordered "blobs" of features. Blobs are differentiably placed onto a feature grid that is decoded into an image by a generative adversarial network. Due to the spatial uniformity of blobs and the locality inherent to convolution, our network learns to associate different blobs with different entities in a scene and to arrange these blobs to capture scene layout. We demonstrate this emergent behavior by showing that, despite training without any supervision, our method enables applications such as easy manipulation of objects within a scene (e.g., moving, removing, and restyling furniture), creation of feasible scenes given constraints (e.g., plausible rooms with drawers at a particular location), and parsing of real-world images into constituent parts. On a challenging multi-category dataset of indoor scenes, BlobGAN outperforms StyleGAN2 in image quality as measured by FID. See our project page for video results and interactive demo: [this https URL](https://www.dave.ml/blobgan).

* **Day 17 (01/17/2022)**: [ConDor: Self-Supervised Canonicalization of 3D Pose for Partial Shapes](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/017%20ConDor.pdf)

**Abstract—** Progress in 3D object understanding has relied on manually canonicalized shape datasets that contain instances with consistent position and orientation (3D pose). This has made it hard to generalize these methods to in-the-wild shapes, eg., from internet model collections or depth sensors. ConDor is a self-supervised method that learns to Canonicalize the 3D orientation and position for full and partial 3D point clouds. We build on top of Tensor Field Networks (TFNs), a class of permutation- and rotation-equivariant, and translation-invariant 3D networks. During inference, our method takes an unseen full or partial 3D point cloud at an arbitrary pose and outputs an equivariant canonical pose. During training, this network uses self-supervision losses to learn the canonical pose from an un-canonicalized collection of full and partial 3D point clouds. ConDor can also learn to consistently co-segment object parts without any supervision. Extensive quantitative results on four new metrics show that our approach outperforms existing methods while enabling new applications such as operation on depth images and annotation transfer.

* **Day 18 (01/18/2022)**: [Dense-Captioning Events in Videos](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/018%20Dense%20Captioning%20Events%20in%20Video.pdf)

**Abstract—** Most natural videos contain numerous events. For example, in a video of a "man playing a piano", the video might also contain "another man dancing" or "a crowd clapping". We introduce the task of dense-captioning events, which involves both detecting and describing events in a video. We propose a new model that is able to identify all events in a single pass of the video while simultaneously describing the detected events with natural language. Our model introduces a variant of an existing proposal module that is designed to capture both short as well as long events that span minutes. To capture the dependencies between the events in a video, our model introduces a new captioning module that uses contextual information from past and future events to jointly describe all events. We also introduce ActivityNet Captions, a large-scale benchmark for dense-captioning events. ActivityNet Captions contains 20k videos amounting to 849 video hours with 100k total descriptions, each with it's unique start and end time. Finally, we report performances of our model for dense-captioning events, video retrieval and localization.

* **Day 19 (01/19/2022)**: [ARTEMIS: Articulated Neural Pets with Appearance and Motion Synthesis](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/019%20Artemis%20Articulated%20Neural%20Pets%20with%20Appearance%20and%20Motion.pdf)

**Abstract—** We, humans, are entering into a virtual era and indeed want to bring animals to the virtual world as well for companion. Yet, computer-generated (CGI) furry animals are limited by tedious off-line rendering, let alone interactive motion control. In this paper, we present ARTEMIS, a novel neural modeling and rendering pipeline for generating ARTiculated neural pets with appEarance and Motion synthesIS. Our ARTEMIS enables interactive motion control, real-time animation, and photo-realistic rendering of furry animals. The core of our ARTEMIS is a neural-generated (NGI) animal engine, which adopts an efficient octree-based representation for animal animation and fur rendering. The animation then becomes equivalent to voxel-level deformation based on explicit skeletal warping. We further use a fast octree indexing and efficient volumetric rendering scheme to generate appearance and density features maps. Finally, we propose a novel shading network to generate high-fidelity details of appearance and opacity under novel poses from appearance and density feature maps. For the motion control module in ARTEMIS, we combine state-of-the-art animal motion capture approach with recent neural character control scheme. We introduce an effective optimization scheme to reconstruct the skeletal motion of real animals captured by a multi-view RGB and Vicon camera array. We feed all the captured motion into a neural character control scheme to generate abstract control signals with motion styles. We further integrate ARTEMIS into existing engines that support VR headsets, providing an unprecedented immersive experience where a user can intimately interact with a variety of virtual animals with vivid movements and photo-realistic appearance. We make available our ARTEMIS model and dynamic furry animal dataset at [this https URL](https://haiminluo.github.io/publication/artemis/).

* **Day 20 (01/20/2022)**: [End-to-End Visual Editing with a Generatively PreTrained Artist](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/020%20End-to-End%20Visual%20Editting%20with%20a%20Generatively%20PreTrained%20Artist.pdf)

**Abstract—** We consider the targeted image editing problem: blending a region in a source image with a driver image that specifies the desired change. Differently from prior works, we solve this problem by learning a conditional probability distribution of the edits, end-to-end. Training such a model requires addressing a fundamental technical challenge: the lack of example edits for training. To this end, we propose a self-supervised approach that simulates edits by augmenting off-the-shelf images in a target domain. The benefits are remarkable: implemented as a state-of-the-art auto-regressive transformer, our approach is simple, sidesteps difficulties with previous methods based on GAN-like priors, obtains significantly better edits, and is efficient. Furthermore, we show that different blending effects can be learned by an intuitive control of the augmentation process, with no other changes required to the model architecture. We demonstrate the superiority of this approach across several datasets in extensive quantitative and qualitative experiments, including human studies, significantly outperforming prior work.

* **Day 21 (01/21/2022)**: [Ensembling Off-the-shelf models for GAN Training](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/021%20Ensembling%20Off-the-shelf%20Models%20for%20GAN%20Training.pdf)

**Abstract—** The advent of large-scale training has produced a cornucopia of powerful visual recognition models. However, generative models, such as GANs, have traditionally been trained from scratch in an unsupervised manner. Can the collective "knowledge" from a large bank of pretrained vision models be leveraged to improve GAN training? If so, with so many models to choose from, which one(s) should be selected, and in what manner are they most effective? We find that pretrained computer vision models can significantly improve performance when used in an ensemble of discriminators. Notably, the particular subset of selected models greatly affects performance. We propose an effective selection mechanism, by probing the linear separability between real and fake samples in pretrained model embeddings, choosing the most accurate model, and progressively adding it to the discriminator ensemble. Interestingly, our method can improve GAN training in both limited data and large-scale settings. Given only 10k training samples, our FID on LSUN Cat matches the StyleGAN2 trained on 1.6M images. On the full dataset, our method improves FID by 1.5x to 2x on cat, church, and horse categories of LSUN.

* **Day 22 (01/22/2022)**: [End-to-End Object Detection with Transformers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/022%20End-to-End%20Object%20Detection%20with%20Transformers.pdf)

**Abstract—** We present a new method that views object detection as a direct set prediction problem. Our approach streamlines the detection pipeline, effectively removing the need for many hand-designed components like a non-maximum suppression procedure or anchor generation that explicitly encode our prior knowledge about the task. The main ingredients of the new framework, called DEtection TRansformer or DETR, are a set-based global loss that forces unique predictions via bipartite matching, and a transformer encoder-decoder architecture. Given a fixed small set of learned object queries, DETR reasons about the relations of the objects and the global image context to directly output the final set of predictions in parallel. The new model is conceptually simple and does not require a specialized library, unlike many other modern detectors. DETR demonstrates accuracy and run-time performance on par with the well-established and highly-optimized Faster RCNN baseline on the challenging COCO object detection dataset. Moreover, DETR can be easily generalized to produce panoptic segmentation in a unified manner. We show that it significantly outperforms competitive baselines. Training code and pretrained models are available at [this https URL](https://github.com/facebookresearch/detr).

* **Day 23 (01/23/2022)**: [A Generalist Agent](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/023%20A%20Generalist%20Agent.pdf)

**Abstract—** Inspired by progress in large-scale language modelling, we apply a similar approach towards building a single generalist agent beyond the realm of text outputs. The agent, which we refer to as Gato, works as a multi-modal, multi-task, multi-embodiment generalist policy. The same network with the same weights can play Atari, caption images, chat, stack blocks with a real robot arm and much more, deciding based on its context whether to output text, joint torques, button presses, or other tokens. In this report we describe the model and the data, and document the current capabilities of Gato.

* **Day 24 (01/24/2022)**: [Differentiable Signed Distance Function Rendering](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/024%20Differentiable%20Signed%20Distance%20Function%20Rendering.pdf)

**Abstract—** Physically-based differentiable rendering has recently emerged as an attractive new technique for solving inverse problems that recover complete 3D scene representations from images. The inversion of shape parameters is of particular interest but also poses severe challenges: shapes are intertwined with visibility, whose discontinuous nature introduces severe bias in computed derivatives unless costly precautions are taken. Shape representations like triangle meshes suffer from additional difficulties, since the continuous optimization of mesh parameters cannot introduce topological changes. One common solution to these difficulties entails representing shapes using signed distance functions (SDFs) and gradually adapting their zero level set during optimization. Previous differentiable rendering of SDFs did not fully account for visibility gradients and required the use of mask or silhouette supervision, or discretization into a triangle mesh. In this article, we show how to extend the commonly used sphere tracing algorithm so that it additionally outputs a reparameterization that provides the means to compute accurate shape parameter derivatives. At a high level, this resembles techniques for differentiable mesh rendering, though we show that the SDF representation admits a particularly efficient reparameterization that outperforms prior work. Our experiments demonstrate the reconstruction of (synthetic) objects without complex regularization or priors, using only a per-pixel RGB loss.

* **Day 25 (01/25/2022)**: [PoseTriplet: Co-evolving 3D Human Pose Estimation, Imitation, and Hallucination under Self-Supervision](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/025%20PoseTriplet%20Co-Evolving%203D%20Human%20Pose%20Estimation%2C%20Imitation%2C%20and%20Hallucination%20under%20Self-Supervision.pdf)

**Abstract—** Existing self-supervised 3D human pose estimation schemes have largely relied on weak supervisions like consistency loss to guide the learning, which, inevitably, leads to inferior results in real-world scenarios with unseen poses. In this paper, we propose a novel self-supervised approach that allows us to explicitly generate 2D-3D pose pairs for augmenting supervision, through a self-enhancing dual-loop learning framework. This is made possible via introducing a reinforcement-learning-based imitator, which is learned jointly with a pose estimator alongside a pose hallucinator; the three components form two loops during the training process, complementing and strengthening one another. Specifically, the pose estimator transforms an input 2D pose sequence to a low-fidelity 3D output, which is then enhanced by the imitator that enforces physical constraints. The refined 3D poses are subsequently fed to the hallucinator for producing even more diverse data, which are, in turn, strengthened by the imitator and further utilized to train the pose estimator. Such a co-evolution scheme, in practice, enables training a pose estimator on self-generated motion data without relying on any given 3D data. Extensive experiments across various benchmarks demonstrate that our approach yields encouraging results significantly outperforming the state of the art and, in some cases, even on par with results of fully-supervised methods. Notably, it achieves 89.1% 3D PCK on MPI-INF-3DHP under self-supervised cross-dataset evaluation setup, improving upon the previous best self-supervised methods by 8.6%. Code can be found at: [this https URL](https://github.com/Garfield-kh/PoseTriplet).

* **Day 26 (01/26/2022)**: [Learned Vertex Descent: A New Direction for 3D Human Model Fitting](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/026%20Learned%20Vertex%20Descent%20A%20New%20Direction%20for%203D%20Human%20Model%20Fitting.pdf)

**Abstract—** We propose a novel optimization-based paradigm for 3D human model fitting on images and scans. In contrast to existing approaches that directly regress the parameters of a low-dimensional statistical body model (e.g. SMPL) from input images, we train an ensemble of per-vertex neural fields network. The network predicts, in a distributed manner, the vertex descent direction towards the ground truth, based on neural features extracted at the current vertex projection. At inference, we employ this network, dubbed LVD, within a gradient-descent optimization pipeline until its convergence, which typically occurs in a fraction of a second even when initializing all vertices into a single point. An exhaustive evaluation demonstrates that our approach is able to capture the underlying body of clothed people with very different body shapes, achieving a significant improvement compared to state-of-the-art. LVD is also applicable to 3D model fitting of humans and hands, for which we show a significant improvement to the SOTA with a much simpler and faster method.

* **Day 27 (01/27/2022)**: [Photorealistic Text-to-Image Diffusion Models with Deep Language Understanding](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/027%20Photorealistic%20TTI%20Diffusion%20Models%20with%20Deep%20Language%20Understanding.pdf)

**Abstract—** We present Imagen, a text-to-image diffusion model with an unprecedented degree of photorealism and a deep level of language understanding. Imagen builds on the power of large transformer language models in understanding text and hinges on the strength of diffusion models in high-fidelity image generation. Our key discovery is that generic large language models (e.g. T5), pretrained on text-only corpora, are surprisingly effective at encoding text for image synthesis: increasing the size of the language model in Imagen boosts both sample fidelity and image-text alignment much more than increasing the size of the image diffusion model. Imagen achieves a new state-of-the-art FID score of 7.27 on the COCO dataset, without ever training on COCO, and human raters find Imagen samples to be on par with the COCO data itself in image-text alignment. To assess text-to-image models in greater depth, we introduce DrawBench, a comprehensive and challenging benchmark for text-to-image models. With DrawBench, we compare Imagen with recent methods including VQ-GAN+CLIP, Latent Diffusion Models, and DALL-E 2, and find that human raters prefer Imagen over other models in side-by-side comparisons, both in terms of sample quality and image-text alignment. See https://imagen.research.google/ for an overview of the results.

* **Day 28 (01/28/2022)**: [Tnt Attacks! Universal Naturalistic Adversarial Patches Against Deep Neural Network Systems](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/028%20TnT%20Attacks!%20Universal%20Naturalistic%20Adversarial%20Patches%20Against%20Deep%20Neural%20Network%20Systems.pdf)

**Abstract—** Deep neural networks are vulnerable to attacks from adversarial inputs and, more recently, Trojans to misguide or hijack the model's decision. We expose the existence of an intriguing class of spatially bounded, physically realizable, adversarial examples -- Universal NaTuralistic adversarial paTches -- we call TnTs, by exploring the superset of the spatially bounded adversarial example space and the natural input space within generative adversarial networks. Now, an adversary can arm themselves with a patch that is naturalistic, less malicious-looking, physically realizable, highly effective achieving high attack success rates, and universal. A TnT is universal because any input image captured with a TnT in the scene will: i) misguide a network (untargeted attack); or ii) force the network to make a malicious decision (targeted attack). Interestingly, now, an adversarial patch attacker has the potential to exert a greater level of control -- the ability to choose a location-independent, natural-looking patch as a trigger in contrast to being constrained to noisy perturbations -- an ability is thus far shown to be only possible with Trojan attack methods needing to interfere with the model building processes to embed a backdoor at the risk discovery; but, still realize a patch deployable in the physical world. Through extensive experiments on the large-scale visual classification task, ImageNet with evaluations across its entire validation set of 50,000 images, we demonstrate the realistic threat from TnTs and the robustness of the attack. We show a generalization of the attack to create patches achieving higher attack success rates than existing state-of-the-art methods. Our results show the generalizability of the attack to different visual classification tasks (CIFAR-10, GTSRB, PubFig) and multiple state-of-the-art deep neural networks such as WideResnet50, Inception-V3 and VGG-16.

* **Day 29 (01/29/2022)**: [Super Vision Transformer](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/029%20Super%20Vision%20Transformer.pdf)

**Abstract—** We attempt to reduce the computational costs in vision transformers (ViTs), which increase quadratically in the token number. We present a novel training paradigm that trains only one ViT model at a time, but is capable of providing improved image recognition performance with various computational costs. Here, the trained ViT model, termed super vision transformer (SuperViT), is empowered with the versatile ability to solve incoming patches of multiple sizes as well as preserve informative tokens with multiple keeping rates (the ratio of keeping tokens) to achieve good hardware efficiency for inference, given that the available hardware resources often change from time to time. Experimental results on ImageNet demonstrate that our SuperViT can considerably reduce the computational costs of ViT models with even performance increase. For example, we reduce 2x FLOPs of DeiT-S while increasing the Top-1 accuracy by 0.2% and 0.7% for 1.5x reduction. Also, our SuperViT significantly outperforms existing studies on efficient vision transformers. For example, when consuming the same amount of FLOPs, our SuperViT surpasses the recent state-of-the-art (SoTA) EViT by 1.1% when using DeiT-S as their backbones. The project of this work is made publicly available at [this https URL](https://github.com/lmbxmu/SuperViT).

* **Day 30 (01/30/2022)**: [Simple Unsupervised Object-Centric Learning for Complex and Naturalistic Videos](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/030%20Simple%20Unsupervised%20Object-Centric%20Learning%20for%20Complex%20and%20Naturalistic%20Videos.pdf)

**Abstract—** Unsupervised object-centric learning aims to represent the modular, compositional, and causal structure of a scene as a set of object representations and thereby promises to resolve many critical limitations of traditional single-vector representations such as poor systematic generalization. Although there have been many remarkable advances in recent years, one of the most critical problems in this direction has been that previous methods work only with simple and synthetic scenes but not with complex and naturalistic images or videos. In this paper, we propose STEVE, an unsupervised model for object-centric learning in videos. Our proposed model makes a significant advancement by demonstrating its effectiveness on various complex and naturalistic videos unprecedented in this line of research. Interestingly, this is achieved by neither adding complexity to the model architecture nor introducing a new objective or weak supervision. Rather, it is achieved by a surprisingly simple architecture that uses a transformer-based image decoder conditioned on slots and the learning objective is simply to reconstruct the observation. Our experiment results on various complex and naturalistic videos show significant improvements compared to the previous state-of-the-art.

* **Day 31 (01/31/2022)**: [Contrastive Learning Rivals Masked Image Modeling in Fine-Tuning via Feature Distillation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/031%20Contrastive%20Learning%20Rivals%20Masked%20Image%20Modeling%20in%20FineTuning%20via%20Feature%20Distillation.pdf)

**Abstract—** Masked image modeling (MIM) learns representations with remarkably good fine-tuning performances, overshadowing previous prevalent pre-training approaches such as image classification, instance contrastive learning, and image-text alignment. In this paper, we show that the inferior fine-tuning performance of these pre-training approaches can be significantly improved by a simple post-processing in the form of feature distillation (FD). The feature distillation converts the old representations to new representations that have a few desirable properties just like those representations produced by MIM. These properties, which we aggregately refer to as optimization friendliness, are identified and analyzed by a set of attention- and optimization-related diagnosis tools. With these properties, the new representations show strong fine-tuning performance. Specifically, the contrastive self-supervised learning methods are made as competitive in fine-tuning as the state-of-the-art masked image modeling (MIM) algorithms. The CLIP models' fine-tuning performance is also significantly improved, with a CLIP ViT-L model reaching 89.0% top-1 accuracy on ImageNet-1K classification. On the 3-billion-parameter SwinV2-G model, the fine-tuning accuracy is improved by +1.5 mIoU / +1.1 mAP to 61.4 mIoU / 64.2 mAP on ADE20K semantic segmentation and COCO object detection, respectively, creating new records on both benchmarks. More importantly, our work provides a way for the future research to focus more effort on the generality and scalability of the learnt representations without being pre-occupied with optimization friendliness since it can be enhanced rather easily. The code will be available at [this https URL](https://github.com/SwinTransformer/Feature-Distillation).

* **Day 32 (02/01/2022)**: [Few-Shot Adaptation of Pre-Trained Networks for Domain Shift](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/032%20Few-Shot%20Adaptation%20of%20Pre-Trained%20Networks%20for%20Domain%20Shift.pdf)

**Abstract—** Deep networks are prone to performance degradation when there is a domain shift between the source (training) data and target (test) data. Recent test-time adaptation methods update batch normalization layers of pre-trained source models deployed in new target environments with streaming data to mitigate such performance degradation. Although such methods can adapt on-the-fly without first collecting a large target domain dataset, their performance is dependent on streaming conditions such as mini-batch size and class-distribution, which can be unpredictable in practice. In this work, we propose a framework for few-shot domain adaptation to address the practical challenges of data-efficient adaptation. Specifically, we propose a constrained optimization of feature normalization statistics in pre-trained source models supervised by a small support set from the target domain. Our method is easy to implement and improves source model performance with as few as one sample per class for classification tasks. Extensive experiments on 5 cross-domain classification and 4 semantic segmentation datasets show that our method achieves more accurate and reliable performance than test-time adaptation, while not being constrained by streaming conditions.

* **Day 33 (02/02/2022)**: [REVIVE: Regional VIsual Representation Matters in KB VQA](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/033%20REVIVE%20Regional%20Visual%20Representation%20Matters%20in%20KB%20VQA.pdf)

**Abstract—** This paper revisits visual representation in knowledge-based visual question answering (VQA) and demonstrates that using regional information in a better way can significantly improve the performance. While visual representation is extensively studied in traditional VQA, it is under-explored in knowledge-based VQA even though these two tasks share the common spirit, i.e., rely on visual input to answer the question. Specifically, we observe that in most state-of-the-art knowledge-based VQA methods: 1) visual features are extracted either from the whole image or in a sliding window manner for retrieving knowledge, and the important relationship within/among object regions is neglected; 2) visual features are not well utilized in the final answering model, which is counter-intuitive to some extent. Based on these observations, we propose a new knowledge-based VQA method REVIVE, which tries to utilize the explicit information of object regions not only in the knowledge retrieval stage but also in the answering model. The key motivation is that object regions and inherent relationships are important for knowledge-based VQA. We perform extensive experiments on the standard OK-VQA dataset and achieve new state-of-the-art performance, i.e., 58.0 state-of-the-art method by a large margin (+3.6 analysis and show the necessity of regional information in different framework components for knowledge-based VQA.

* **Day 34 (02/03/2022)**: [SAMURAI: Shape And Material from Unconstrained Real-World Arbitrary Image Collections](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/034%20SAMURAI%20Shape%20And%20Material%20from%20Unconstrained%20Real-World%20Arbitrary%20Image%20Collections.pdf)

**Abstract—** Inverse rendering of an object under entirely unknown capture conditions is a fundamental challenge in computer vision and graphics. Neural approaches such as NeRF have achieved photorealistic results on novel view synthesis, but they require known camera poses. Solving this problem with unknown camera poses is highly challenging as it requires joint optimization over shape, radiance, and pose. This problem is exacerbated when the input images are captured in the wild with varying backgrounds and illuminations. Standard pose estimation techniques fail in such image collections in the wild due to very few estimated correspondences across images. Furthermore, NeRF cannot relight a scene under any illumination, as it operates on radiance (the product of reflectance and illumination). We propose a joint optimization framework to estimate the shape, BRDF, and per-image camera pose and illumination. Our method works on in-the-wild online image collections of an object and produces relightable 3D assets for several use-cases such as AR/VR. To our knowledge, our method is the first to tackle this severely unconstrained task with minimal user interaction. Project page: [this https URL](https://markboss.me/publication/2022-samurai/) Video: [this https URL](https://youtu.be/LlYuGDjXp-8)

* **Day 35 (02/04/2022)**: [Decomposing NeRF For Editing via Feature Field Distillation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/035%20Decomposing%20NERF%20for%20Editing%20via%20Feature%20Field%20Distillation.pdf)

**Abstract—** Emerging neural radiance fields (NeRF) are a promising scene representation for computer graphics, enabling high-quality 3D reconstruction and novel view synthesis from image observations. However, editing a scene represented by a NeRF is challenging, as the underlying connectionist representations such as MLPs or voxel grids are not object-centric or compositional. In particular, it has been difficult to selectively edit specific regions or objects. In this work, we tackle the problem of semantic scene decomposition of NeRFs to enable query-based local editing of the represented 3D scenes. We propose to distill the knowledge of off-the-shelf, self-supervised 2D image feature extractors such as CLIP-LSeg or DINO into a 3D feature field optimized in parallel to the radiance field. Given a user-specified query of various modalities such as text, an image patch, or a point-and-click selection, 3D feature fields semantically decompose 3D space without the need for re-training and enable us to semantically select and edit regions in the radiance field. Our experiments validate that the distilled feature fields (DFFs) can transfer recent progress in 2D vision and language foundation models to 3D scene representations, enabling convincing 3D segmentation and selective editing of emerging neural graphics representations.

* **Day 36 (02/05/2022)**: [RTMV: A Ray-Traced Multi-View Synthetic Dataset for Novel View Synthesis](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/036%20RTMV%20A%20Ray-Traced%20Multi-View%20Synthetic%20Dataset%20for%20Novel%20View%20Synthesis.pdf)

**Abstract—** We present a large-scale synthetic dataset for novel view synthesis consisting of ~300k images rendered from nearly 2000 complex scenes using high-quality ray tracing at high resolution (1600 x 1600 pixels). The dataset is orders of magnitude larger than existing synthetic datasets for novel view synthesis, thus providing a large unified benchmark for both training and evaluation. Using 4 distinct sources of high-quality 3D meshes, the scenes of our dataset exhibit challenging variations in camera views, lighting, shape, materials, and textures. Because our dataset is too large for existing methods to process, we propose Sparse Voxel Light Field (SVLF), an efficient voxel-based light field approach for novel view synthesis that achieves comparable performance to NeRF on synthetic data, while being an order of magnitude faster to train and two orders of magnitude faster to render. SVLF achieves this speed by relying on a sparse voxel octree, careful voxel sampling (requiring only a handful of queries per ray), and reduced network structure; as well as ground truth depth maps at training time. Our dataset is generated by NViSII, a Python-based ray tracing renderer, which is designed to be simple for non-experts to use and share, flexible and powerful through its use of scripting, and able to create high-quality and physically-based rendered images. Experiments with a subset of our dataset allow us to compare standard methods like NeRF and mip-NeRF for single-scene modeling, and pixelNeRF for category-level modeling, pointing toward the need for future improvements in this area.

* **Day 37 (02/06/2022)**: [View Synthesis using Sculpted Neural Points](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/037%20View%20Synthesis%20using%20Sculpted%20Neural%20Points.pdf)

**Abstract—** We address the task of view synthesis, which can be posed as recovering a rendering function that renders new views from a set of existing images. In many recent works such as NeRF, this rendering function is parameterized using implicit neural representations of scene geometry. Implicit neural representations have achieved impressive visual quality but have drawbacks in computational efficiency. In this work, we propose a new approach that performs view synthesis using point clouds. It is the first point-based method to achieve better visual quality than NeRF while being more than 100x faster in rendering speed. Our approach builds on existing works on differentiable point-based rendering but introduces a novel technique we call "Sculpted Neural Points (SNP)", which significantly improves the robustness to errors and holes in the reconstructed point cloud. Experiments show that on the task of view synthesis, our sculpting technique closes the gap between point-based and implicit representation-based methods. Code is available at [this https URL](https://github.com/princeton-vl/SNP) and supplementary video at [this https URL](https://youtu.be/dBwCQP9uNws).

* **Day 38 (02/07/2022)**: [PREF: Phasorial Embedding Fields for Compact Neural Representations](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/038%20PREF%20Phasorial%20Embedding%20Fields%20for%20Compact%20Neural%20Representations.pdf)
 
**Abstract—** We present a phasorial embedding field \emph{PREF} as a compact representation to facilitate neural signal modeling and reconstruction tasks. Pure multi-layer perceptron (MLP) based neural techniques are biased towards low frequency signals and have relied on deep layers or Fourier encoding to avoid losing details. PREF instead employs a compact and physically explainable encoding field based on the phasor formulation of the Fourier embedding space. We conduct comprehensive experiments to demonstrate the advantages of PREF over the latest spatial embedding techniques. We then develop a highly efficient frequency learning framework using an approximated inverse Fourier transform scheme for PREF along with a novel Parseval regularizer. Extensive experiments show our efficient and compact frequency-based neural signal processing technique is on par with and even better than the state-of-the-art in 2D image completion, 3D SDF surface regression, and 5D radiance field reconstruction.

* **Day 39 (02/08/2022)**: [Generating Long Videos of Dynamic Scenes](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/039%20Generating%20Long%20Videos%20of%20Dynamic%20Scenes.pdf)
 
**Abstract—** We present a video generation model that accurately reproduces object motion, changes in camera viewpoint, and new content that arises over time. Existing video generation methods often fail to produce new content as a function of time while maintaining consistencies expected in real environments, such as plausible dynamics and object persistence. A common failure case is for content to never change due to over-reliance on inductive biases to provide temporal consistency, such as a single latent code that dictates content for the entire video. On the other extreme, without long-term consistency, generated videos may morph unrealistically between different scenes. To address these limitations, we prioritize the time axis by redesigning the temporal latent representation and learning long-term consistency from data by training on longer videos. To this end, we leverage a two-phase training strategy, where we separately train using longer videos at a low resolution and shorter videos at a high resolution. To evaluate the capabilities of our model, we introduce two new benchmark datasets with explicit focus on long-term temporal dynamics.

* **Day 40 (02/09/2022)**: [Conditional Adversarial Synthesis of 3D Facial Action Units](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/040%20Conditional%20Adversarial%20Synthesis%20of%203D%20Facial%20Action%20Units.pdf)

**Abstract—** Employing deep learning-based approaches for fine-grained facial expression analysis, such as those involving the estimation of Action Unit (AU) intensities, is difficult due to the lack of a large-scale dataset of real faces with sufficiently diverse AU labels for training. In this paper, we consider how AU-level facial image synthesis can be used to substantially augment such a dataset. We propose an AU synthesis framework that combines the well-known 3D Morphable Model (3DMM), which intrinsically disentangles expression parameters from other face attributes, with models that adversarially generate 3DMM expression parameters conditioned on given target AU labels, in contrast to the more conventional approach of generating facial images directly. In this way, we are able to synthesize new combinations of expression parameters and facial images from desired AU labels. Extensive quantitative and qualitative results on the benchmark DISFA dataset demonstrate the effectiveness of our method on 3DMM facial expression parameter synthesis and data augmentation for deep learning-based AU intensity estimation.

* **Day 41 (02/10/2022)**: [Efficient Geometry-aware 3D Generative Adversarial Networks](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/041%20Efficient%20Geometry-aware%203D%20Generative%20Adversarial%20Networks.pdf)

**Abstract—** Unsupervised generation of high-quality multi-view-consistent images and 3D shapes using only collections of single-view 2D photographs has been a long-standing challenge. Existing 3D GANs are either compute-intensive or make approximations that are not 3D-consistent; the former limits quality and resolution of the generated images and the latter adversely affects multi-view consistency and shape quality. In this work, we improve the computational efficiency and image quality of 3D GANs without overly relying on these approximations. We introduce an expressive hybrid explicit-implicit network architecture that, together with other design choices, synthesizes not only high-resolution multi-view-consistent images in real time but also produces high-quality 3D geometry. By decoupling feature generation and neural rendering, our framework is able to leverage state-of-the-art 2D CNN generators, such as StyleGAN2, and inherit their efficiency and expressiveness. We demonstrate state-of-the-art 3D-aware synthesis with FFHQ and AFHQ Cats, among other experiments.

* **Day 42 (02/11/2022)**: [An Improved One millisecond Mobile Backbone](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/042%20An%20Improved%20One%20millisecond%20Mobile%20Backbone.pdf)

**Abstract—** Efficient neural network backbones for mobile devices are often optimized for metrics such as FLOPs or parameter count. However, these metrics may not correlate well with latency of the network when deployed on a mobile device. Therefore, we perform extensive analysis of different metrics by deploying several mobile-friendly networks on a mobile device. We identify and analyze architectural and optimization bottlenecks in recent efficient neural networks and provide ways to mitigate these bottlenecks. To this end, we design an efficient backbone MobileOne, with variants achieving an inference time under 1 ms on an iPhone12 with 75.9% top-1 accuracy on ImageNet. We show that MobileOne achieves state-of-the-art performance within the efficient architectures while being many times faster on mobile. Our best model obtains similar performance on ImageNet as MobileFormer while being 38x faster. Our model obtains 2.3% better top-1 accuracy on ImageNet than EfficientNet at similar latency. Furthermore, we show that our model generalizes to multiple tasks - image classification, object detection, and semantic segmentation with significant improvements in latency and accuracy as compared to existing efficient architectures when deployed on a mobile device.

* **Day 43 (02/12/2022)**: [Position Labels for Self-Supervised Vision Transformer](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/043%20Position%20Labels%20for%20Self-Supervised%20Vision%20Transformer.pdf)

**Abstract—** Positional encoding is important for vision transformer (ViT) to capture the spatial structure of the input image. General effectiveness has been proven in ViT. In our work we propose to train ViT to recognize the positional label of patches of the input image, this apparently simple task actually yields a meaningful self-supervisory task. Based on previous work on ViT positional encoding, we propose two positional labels dedicated to 2D images including absolute position and relative position. Our positional labels can be easily plugged into various current ViT variants. It can work in two ways: (a) As an auxiliary training target for vanilla ViT (e.g., ViT-B and Swin-B) for better performance. (b) Combine the self-supervised ViT (e.g., MAE) to provide a more powerful self-supervised signal for semantic feature learning. Experiments demonstrate that with the proposed self-supervised methods, ViT-B and Swin-B gain improvements of 1.20% (top-1 Acc) and 0.74% (top-1 Acc) on ImageNet, respectively, and 6.15% and 1.14% improvement on Mini-ImageNet.

* **Day 44 (02/13/2022)**: [Spatial Cross-Attention Improves Self-Supervised Visual Representation Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/044%20Spatial%20Cross-Attention%20Improves%20Self-Supervised%20Visual%20Representation%20Learning.pdf)

**Abstract—** Unsupervised representation learning methods like SwAV are proved to be effective in learning visual semantics of a target dataset. The main idea behind these methods is that different views of a same image represent the same semantics. In this paper, we further introduce an add-on module to facilitate the injection of the knowledge accounting for spatial cross correlations among the samples. This in turn results in distilling intra-class information including feature level locations and cross similarities between same-class instances. The proposed add-on can be added to existing methods such as the SwAV. We can later remove the add-on module for inference without any modification of the learned weights. Through an extensive set of empirical evaluations, we verify that our method yields an improved performance in detecting the class activation maps, top-1 classification accuracy, and down-stream tasks such as object detection, with different configuration settings.

* **Day 45 (02/14/2022)**: [Image Degeneration with Multi-Model Priors Using Denoising Diffusion Probabilistic Models](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/045%20Image%20Degeneration%20with%20Multi-Modal%20Priors%20Using%20Denoising%20Diffusion%20Probabilistic%20Models.pdf)

**Abstract—** Image synthesis under multi-modal priors is a useful and challenging task that has received increasing attention in recent years. A major challenge in using generative models to accomplish this task is the lack of paired data containing all modalities (i.e. priors) and corresponding outputs. In recent work, a variational auto-encoder (VAE) model was trained in a weakly supervised manner to address this challenge. Since the generative power of VAEs is usually limited, it is difficult for this method to synthesize images belonging to complex distributions. To this end, we propose a solution based on a denoising diffusion probabilistic models to synthesise images under multi-model priors. Based on the fact that the distribution over each time step in the diffusion model is Gaussian, in this work we show that there exists a closed-form expression to the generate the image corresponds to the given modalities. The proposed solution does not require explicit retraining for all modalities and can leverage the outputs of individual modalities to generate realistic images according to different constraints. We conduct studies on two real-world datasets to demonstrate the effectiveness of our approach.

* **Day 46 (02/15/2022)**: [SimVP: Simpler yet Better Video Prediction](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/046%20SimVP%20Simpler%20yet%20Better%20Video%20Prediction.pdf)

**Abstract—** From CNN, RNN, to ViT, we have witnessed remarkable advancements in video prediction, incorporating auxiliary inputs, elaborate neural architectures, and sophisticated training strategies. We admire these progresses but are confused about the necessity: is there a simple method that can perform comparably well? This paper proposes SimVP, a simple video prediction model that is completely built upon CNN and trained by MSE loss in an end-to-end fashion. Without introducing any additional tricks and complicated strategies, we can achieve state-of-the-art performance on five benchmark datasets. Through extended experiments, we demonstrate that SimVP has strong generalization and extensibility on real-world datasets. The significant reduction of training cost makes it easier to scale to complex scenarios. We believe SimVP can serve as a solid baseline to stimulate the further development of video prediction. The code is available at [this https URL](https://github.com/gaozhangyang/SimVP-Simpler-yet-Better-Video-Prediction).

* **Day 47 (02/16/2022)**: [Saccade Mechanisms for Image Classification, Object Detection and Tracking](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/047%20Saccade%20Mechanisms%20for%20Image%20Classification%20Object%20Detection%20and%20Tracking.pdf)

**Abstract—** We examine how the saccade mechanism from biological vision can be used to make deep neural networks more efficient for classification and object detection problems. Our proposed approach is based on the ideas of attention-driven visual processing and saccades, miniature eye movements influenced by attention. We conduct experiments by analyzing: i) the robustness of different deep neural network (DNN) feature extractors to partially-sensed images for image classification and object detection, and ii) the utility of saccades in masking image patches for image classification and object tracking. Experiments with convolutional nets (ResNet-18) and transformer-based models (ViT, DETR, TransTrack) are conducted on several datasets (CIFAR-10, DAVSOD, MSCOCO, and MOT17). Our experiments show intelligent data reduction via learning to mimic human saccades when used in conjunction with state-of-the-art DNNs for classification, detection, and tracking tasks. We observed minimal drop in performance for the classification and detection tasks while only using about 30\% of the original sensor data. We discuss how the saccade mechanism can inform hardware design via ``in-pixel'' processing.

* **Day 48 (02/17/2022)**: [Globally-Optimal Contrast Maximisation for Event Cameras](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/048%20Globally-Optimal%20Contrast%20Maximisation%20for%20Event%20Cameras.pdf)

**Abstract—** Event cameras are bio-inspired sensors that perform well in challenging illumination conditions and have high temporal resolution. However, their concept is fundamentally different from traditional frame-based cameras. The pixels of an event camera operate independently and asynchronously. They measure changes of the logarithmic brightness and return them in the highly discretised form of time-stamped events indicating a relative change of a certain quantity since the last event. New models and algorithms are needed to process this kind of measurements. The present work looks at several motion estimation problems with event cameras. The flow of the events is modelled by a general homographic warping in a space-time volume, and the objective is formulated as a maximisation of contrast within the image of warped events. Our core contribution consists of deriving globally optimal solutions to these generally non-convex problems, which removes the dependency on a good initial guess plaguing existing methods. Our methods rely on branch-and-bound optimisation and employ novel and efficient, recursive upper and lower bounds derived for six different contrast estimation functions. The practical validity of our approach is demonstrated by a successful application to three different event camera motion estimation problems.

* **Day 49 (02/18/2022)**: [Real-time Hyper-Dimensional Reconfiguration at the Edge using Hardware Accelerators](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/049%20Real-time%20Hyper-Dimensional%20Reconfiguration%20at%20the%20Edge%20using%20Hardware%20Accelerators.pdf) 

**Abstract—** In this paper we present Hyper-Dimensional Reconfigurable Analytics at the Tactical Edge (HyDRATE) using low-SWaP embedded hardware that can perform real-time reconfiguration at the edge leveraging non-MAC (free of floating-point MultiplyACcumulate operations) deep neural nets (DNN) combined with hyperdimensional (HD) computing accelerators. We describe the algorithm, trained quantized model generation, and simulated performance of a feature extractor free of multiply-accumulates feeding a hyperdimensional logic-based classifier. Then we show how performance increases with the number of hyperdimensions. We describe the realized low-SWaP FPGA hardware and embedded software system compared to traditional DNNs and detail the implemented hardware accelerators. We discuss the measured system latency and power, noise robustness due to use of learnable quantization and HD computing, actual versus simulated system performance for a video activity classification task and demonstration of reconfiguration on this same dataset. We show that reconfigurability in the field is achieved by retraining only the feed-forward HD classifier without gradient descent backpropagation (gradient-free), using few-shot learning of new classes at the edge. Initial work performed used LRCN DNN and is currently extended to use Two-stream DNN with improved performance.

* **Day 50 (02/19/2022)**: [Referring Image Matting](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/050%20Referring%20Image%20Matting.pdf)

**Abstract—** Image matting refers to extracting the accurate foregrounds in the image. Current automatic methods tend to extract all the salient objects in the image indiscriminately. In this paper, we propose a new task named Referring Image Matting (RIM), referring to extracting the meticulous alpha matte of the specific object that can best match the given natural language description. However, prevalent visual grounding methods are all limited to the segmentation level, probably due to the lack of high-quality datasets for RIM. To fill the gap, we establish the first large-scale challenging dataset RefMatte by designing a comprehensive image composition and expression generation engine to produce synthetic images on top of current public high-quality matting foregrounds with flexible logics and re-labelled diverse attributes. RefMatte consists of 230 object categories, 47,500 images, 118,749 expression-region entities, and 474,996 expressions, which can be further extended easily in the future. Besides this, we also construct a real-world test set with manually generated phrase annotations consisting of 100 natural images to further evaluate the generalization of RIM models. We first define the task of RIM in two settings, i.e., prompt-based and expression-based, and then benchmark several representative methods together with specific model designs for image matting. The results provide empirical insights into the limitations of existing methods as well as possible solutions. We believe the new task RIM along with the RefMatte dataset will open new research directions in this area and facilitate future studies. The dataset and code will be made publicly available at [this https URL](https://github.com/JizhiziLi/RIM).

* **Day 51 (02/20/2022)**: [MEAT: Maneuver Extraction from Agent Trajectories](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/051%20MEAT%20Maneuver%20Extraction%20from%20Agent%20Trajectories.pdf)

* **Day 52 (02/21/2022)**: [An Image Processing Pipeline for Camera Trap Time-Lapse Recordings](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/052%20An%20Image%20Processing%20Pipeline%20for%20Camera%20Trap%20Time-Lapse%20Recordings.pdf)

* **Day 53 (02/22/2022)**: [Exploring Feature Self-relation for Self-Supervised Transformer](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/053%20Exploring%20Feature%20Self-relation%20for%20Self-Supervised%20Transformer.pdf)

* **Day 54 (02/23/2022)**: [Learning the Space of Deep Models](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/054%20Learning%20the%20Space%20of%20Deep%20Models.pdf)

* **Day 55 (02/24/2022)**: [ClamNet Using Contrastive Learning with Variable Depth UNets for Medical Image Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/055%20ClamNet%20Using%20Contrastive%20Learning%20with%20Variable%20Depth%20UNets%20for%20Medical%20Image%20Segmentation.pdf)

* **Day 56 (02/25/2022)**: [Lost in Transmission: On the Imact of Networking Corruptions on Video ML Models](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/056%20Lost%20in%20Transmission%20On%20the%20Impact%20of%20Networking%20Corruptions%20on%20Video%20ML%20Models.pdf)

* **Day 57 (02/26/2022)**: [Rethinking Spatial Invariance of Convolutional Networks for Object Counting](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/057%20Rethinking%20Spatial%20Invariance%20of%20Convolutional%20Networks%20for%20Object%20Counting.pdf)

* **Day 58 (02/27/2022)**: [Explaining Image Classifiers using Contrastive Counterfactuals in Generative Latent Space](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/058%20Explaining%20Image%20Classifiers%20using%20Contrastive%20Counterfactuals%20in%20Generative%20Latent%20Spaces.pdf)

* **Day 59 (02/28/2022)**: [V4D: Voxel for 4D Novel View Synthesis](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/059%20V4D%20Voxel%20for%204D%20Novel%20View%20Synthesis.pdf)

* **Day 60 (03/01/2022)**: [Compressible-composable NeRF via Rank-residual Decomposition](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/060%20Compressible-composable%20NeRF%20via%20Rank-residual%20Decomposition.pdf)

* **Day 61 (03/02/2022)**: [Novel View Synthesis for High-fidelity Headshot Scenes](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/061%20Novel%20View%20Synthesis%20for%20High-fidelity%20Headshot%20Scenes.pdf)

* **Day 62 (03/03/2022)**: [Fast Dynamic Radiance Fields with Time-Aware Neural Voxels](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/062%20Fast%20Dynamic%20Radiance%20Fields%20with%20Time-Aware%20Neural%20Voxels.pdf)

* **Day 63 (03/04/2022)**: [Neural Volumetric Object Selection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/063%20Neural%20Volumetric%20Object%20Selection.pdf)

* **Day 64 (03/05/2022)**: [D2NRF: Self-Supervised Decoupling of Dynamic and Static Objects from a Monocular Video](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/064%20D2NRF%20Self-Supervised%20Decoupling%20of%20Dynamic%20and%20Static%20Objects%20from%20a%20Monocular%20Video.pdf)

* **Day 65 (03/06/2022)**: [EfficientNeRF: EfficientNeural Radiance Fields](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/065%20EfficientNeRF%20Efficient%20Neural%20Radiance%20Fields.pdf)

* **Day 66 (03/07/2022)**: [Points2NeRF: Generating Neural Radiance Fields from 3D Point Cloud](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/066%20Points2NeRF%20Generating%20Neural%20Radiance%20Fields%20from%203D%20Point%20Cloud.pdf)

* **Day 67 (03/08/2022)**: [Reinforcement Learning with Neural Radiance Fields](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/067%20Reinforcement%20Learning%20with%20Neural%20Radiance%20Fields.pdf)

* **Day 68 (03/09/2022)**: [OBPOSE: Leveraging Canonical Pose for Object-Centric Scene Inference in 3D](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/068%20OBPOSE%20Leveraging%20Canonical%20Pose%20for%20Object-Centric%20Scene%20Inference%20in%203D.pdf)

* **Day 69 (03/10/2022)**: [SNAKE: Shape-aware Neural 3D Keypoint Field](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/069%20SNAKE%20Shape-aware%20Neural%203D%20Keypoint%20Field.pdf)

* **Day 70 (03/11/2022)**: [Beyond RGB: Scene-Property Synthesis with Neural Radiance Fields](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/070%20Beyond%20RGB%20Scene-Property%20Synthesis%20with%20Neural%20Radiance%20Fields.pdf)

* **Day 71 (03/12/2022)**: [Face  Alignment in Full Pose Range: A 3D Total Solution](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/071%20Face%20Alignment%20in%20Full%20Pose%20Range%20A%203D%20Total%20Solution.pdf)

* **Day 72 (03/13/2022)**: [MINER: Multiscale Implicit Neural Representations](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/072%20MINER%20Multiscale%20Implicit%20Neural%20Representations.pdf)

* **Day 73 (03/14/2022)**: [Efficient Geometry-aware 3D Generative Adversarial Networks](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/073%20Efficient%20Geometry-aware%203D%20Generative%20Adversarial%20Networks.pdf)

* **Day 74 (03/15/2022)**: [Zero-Shot and Few-Shot Learning for Lung Cancer Multi-Label Classification using Vision Transformer](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/074%20Zero-Shot%20and%20Few-Shot%20Learning%20for%20Lung%20Cancer%20Multi-label%20Classification%20using%20Vision%20Transformer.pdf)

* **Day 75 (03/16/2022)**: [3DLG-Detectory 3D Object Detection via Simultaneous Local-Global Feature Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/075%203DLGDetector%203D%20Object%20Detection%20via%20Simultaneous%20Local-Global%20Feature%20Learning.pdf)

* **Day 76 (03/17/2022)**: [GraphWalks: Efficient Shape Agnostic Geodesic Shortest Path Estimation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/076%20GraphWalks%20Efficient%20Shape%20Agnostic%20Geodesic%20Shortest%20Path%20Estimation.pdf)

* **Day 77 (03/18/2022)**: [Ray Priors through Reprojection: Improving Neural Radiance Fields for Novel View Extrapolation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/077%20Ray%20Priors%20through%20Reprojection%20Improving%20Neural%20Radiance%20Fields%20for%20Novel%20View%20Extrapolation.pdf)

* **Day 78 (03/19/2022)**: [BodyMap: Learning Full-Body Dense Correspondence Map](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/078%20BodyMap%20Learning%20Full-Body%20Dense%20Correspondence%20Map.pdf)

* **Day 79 (03/20/2022)**: [A 3D Face Model for Pose and Illumination Invariant Face Recognition](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/079%20A%203D%20Face%20Model%20for%20Pose%20and%20Illumination%20Invariant%20Face%20Recognition.pdf)

* **Day 80 (03/21/2022)**: [Automated 3D Face Reconstruction from Multiple Images using Quality Measures](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/080%20Automated%203D%20Face%20Reconstruction%20from%20Multiple%20Images%20using%20Quality%20Measures.pdf)

* **Day 81 (03/22/2022)**: [Fast Neural-Network-based solving of Partial Differential Equations](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/081%20Fast%20Neural%20Network%20based%20solving%20of%20Partial%20Differential%20Equations.pdf)

* **Day 82 (03/23/2022)**: [BEVerse: Unified Perception and Prediction in Birds-Eye-View for Vision Centric Autonomouus Driving](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/082%20BEVerse%20Unified%20Perception%20and%20Prediction%20in%20Birds-Eye-View%20for%20Vision-Centric%20Autonomous%20Driving.pdf)

* **Day 83 (03/24/2022)**: [Learning to Aggregate and Personalize 3D Face From In-The-Wild Photo Collection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/083%20Learning%20to%20Aggregate%20and%20Personalize%203D%20Face%20from%20In-The-Wild%20Photo%20Collection.pdf)

* **Day 84 (03/25/2022)**: [Learning Unbiased Representations via Mutual Information Backpropagation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/084%20Learning%20Unbiased%20Representations%20via%20Mutual%20Information%20Backpropagation.pdf)

* **Day 85 (03/26/2022)**: [Non-Linear 3D Face Morphable Model](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/085%20Nonlinear%203D%20Face%20Morphable%20Model.pdf)

* **Day 86 (03/27/2022)**: [NeRF-In: Free-Form NeRF Inpainting with RGB-D Priors](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/086%20NeRF-In%20Free-Form%20NeRF%20Inpainting%20with%20RGB-D%20Priors.pdf)

* **Day 87 (03/28/2022)**: [Generalizable Neural Radiance Fields for Novel View Synthesis with Transformers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/087%20Generalizable%20Neural%20Radiance%20Fields%20for%20Novel%20View%20Synthesis%20with%20Transformer.pdf)

* **Day 88 (03/29/2022)**: [AR-NeRF: Unsupervised Learning of Depth and Defocus Effects from Natural Images with Aperture Rendering Neural Radiance Fields](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/088%20AR-NeRF%20Unsupervised%20Learning%20of%20Depth%20and%20Defocus%20Effects%20from%20Natural%20Images%20with%20Aperture%20Rendering%20NeRFs.pdf)

* **Day 89 (03/30/2022)**: [SNeS: Learning Probably Symmetric Neural Surfaces from Incomplete Data](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/089%20SNeS%20Learning%20Probably%20Symmetric%20Neural%20Surfaces%20from%20Incomplete%20Data.pdf)

* **Day 90 (03/31/2022)**: [RigNeRF: Fully-Controllable Neural 3D Portraits](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/090%20RigNeRF%20Fully%20Controllable%20Neural%203D%20Portraits.pdf)

* **Day 91 (04/01/2022)**: [Physics Informed Neural Fields for Smoke Reconstruction with Sparse Data](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/091%20Physics%20Informed%20Neural%20Fields%20for%20Smoke%20Reconstruction%20with%20Sparse%20Data.pdf)

* **Day 92 (04/02/2022)**: [GRAM-HD: 3D-Consistent Image Generation at High-Resolution with Generative Radiance Manifolds](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/092%20GRAM-HD%203D-Consistent%20Image%20Generation%20at%20HIgh-Resolution%20with%20Generative%20Radiance%20Manifolds.pdf)

* **Day 93 (04/03/2022)**: [VoxGRAF: Fast 3D-Aware Image Synthesis with Sparse Voxel Grids](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/093%20VoxGRAF%20Fast%203D-Aware%20Image%20Synthesis%20with%20Sparse%20Voxel%20Grids.pdf)

* **Day 94 (04/04/2022)**: [Neural Deformable Voxel Grid for Fast Optimization of Synamic View Synthesis](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/094%20Neural%20Deformable%20Voxel%20Grid%20for%20Fast%20Optimization%20of%20Dynamic%20View%20Synthesis.pdf)

* **Day 95 (04/05/2022)**: [Variable Bitrate Neural Fields](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/095%20Variable%20Bitrate%20Neural%20Fields.pdf)

* **Day 96 (04/06/2022)**: [FWD: Real-time Novel-View Synthesis with Forward Warping and Depth](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/096%20FWD%20Real-time%20Novel%20View%20Synthesis%20with%20Forward%20Warping%20and%20Depth.pdf)

* **Day 97 (04/07/2022)**: [PolyU-BPCoMa: A Dataset and Benchmark Towards Mobile Colorized Mapping Using a Backpack Multisensorial System](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/097%20PolyU-BPCoMa%20A%20Dataset%20and%20Benchmark%20Towards%20Mobile%20Colorized%20Mapping%20Using%20a%20Backpack%20Multisnesorial%20System.pdf)

* **Day 98 (04/08/2022)**: [How to Reduce Change Detection to Semantic Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/098%20How%20to%20Reduce%20Change%20Detection%20to%20Semantic%20Segmentation.pdf)

* **Day 99 (04/09/2022)**: [Real3d-Aug: Point-Cloud Augmentation by Placing Real Objects with Occlusion Handling for 3D Detection and Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/099%20Real3D-Aug%20Point%20Cloud%20Augmentation%20by%20Placing%20Real%20Objects%20with%20Occlusion%20Handling%20for%203D%20Detection%20and%20Segmentation.pdf)

* **Day 100 (04/10/2022)**: [SP-ViT: Learning 3D Spatial Priors for Vision Transformers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/100%20SP-ViT%20Learning%202D%20Spatial%20Priors%20for%20Vision%20Transformers.pdf)

* **Day 101 (04/11/2022)**: [AVATAR: Unconstrained Audiovisual Speech Recognition](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/101%20AVATAR%20Unconstrained%20Audiovisual%20Speech%20Recognition.pdf)

* **Day 102 (04/12/2022)**: [Residual Sparsity Connection Learning for Efficient Video Super-Resolution](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/102%20Residual%20Sparsity%20Connection%20Learning%20for%20Efficient%20Video%20Super-Resolution.pdf)
	
* **Day 103 (04/13/2022)**: [ELUDE: Generating interpretable explanations via a decomposition into labelled and unlabelled features](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/103%20ELUDE%20Generating%20interpretable%20explanations%20via%20a%20decomposition%20into%20labelled%20and%20unlabelled%20features.pdf)

* **Day 104 (04/14/2022)**: [Diffusion Models for Video Prediction and Infilling](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/104%20Diffusion%20Models%20for%20Video%20Prediction%20and%20Infilling.pdf)

* **Day 105 (04/15/2022)**: [Edge Inference with Fully Differentiable Quantized Mixed Precision Neural Networks](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/105%20Edge%20Inference%20with%20Fully%20Differentiable%20Quantized%20Mixed%20Precision%20Neural%20Networks.pdf)

* **Day 106 (04/16/2022)**: [Reconstructing Training Data from Trained Neural Networks](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/106%20Reconstructing%20Training%20Data%20from%20Trained%20Neural%20Networks.pdf)

* **Day 107 (04/17/2022)**: [MoDi: Unconditional Motion Synthesis from Diverse Data](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/107%20MoDi%20Unconditional%20Motion%20Synthesis%20from%20Diverse%20Data.pdf)

* **Day 108 (04/18/2022)**: [Multi-View Imputation and Cross-Attention Network Based on Incomplete Longitudinal and Multi-Modal Data for Alzheimer's Disease Prediction](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/108%20Multi-View%20Imputation%20and%20Cross-Attention%20Network%20Based%20on%20Incomplete%20Longitudinal%20and%20Multi-Modal%20Data%20for%20Alzheimer's%20Disease%20Prediction.pdf)

* **Day 109 (04/19/2022)**: [AMOS: A Large-Scale Abdominal Multi-Organ Benchmark for Versatile Medical Image Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/109%20AMOS%20A%20Large-Scale%20Abdominal%20Multi-Organ%20Benchmark%20for%20Versatile%20Medical%20Image%20Segmentation.pdf)

* **Day 110 (04/20/2022)**: [Learning Effect of Lay People in Gesture-Based Locomotion in Virtual Reality](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/110%20Learning%20Effect%20of%20Lay%20People%20in%20Gesture-Based%20Locomotion%20in%20Virtual%20Reality.pdf)

* **Day 111 (04/21/2022)**: [Neural Scene Representation for Locomotion on Structured Terrain](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/111%20Neural%20Scene%20Representation%20for%20Locomotion%20on%20Structured%20Terrain.pdf)
	
* **Day 112 (04/22/2022)**: [U-PET: MRI-based Dementia Detection with Joint Generation of Synthetic FDG-PET Images](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/112%20U-PET%20MRI-based%20Dementia%20Detection%20with%20Joint%20Generation%20of%20Synthetic%20FDG-PET%20Images.pdf)
	
* **Day 113 (04/23/2022)**: [Longitudinal Detection of New MS Lesions using Deep Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/113%20Longitudinal%20Detection%20of%20New%20MS%20Lesions%20using%20Deep%20Learning.pdf)
	
* **Day 114 (04/24/2022)**: [Video Capsule Endoscopy Classification using Focal Modulation Guided Convolutional Neural Network](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/114%20Video%20Capsule%20Endoscopy%20Classification%20using%20Focal%20Modulation%20Guided%20Convolutional%20Neural%20Network.pdf)
	
* **Day 115 (04/25/2022)**: [SoundSpaces 2.0: A Simulation Platform for Visual-Acoustic Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/115%20SoundSpaces%202.0%20A%20Simulation%20Platform%20for%20Visual-Acoustic%20Learning.pdf)
	
* **Day 116 (04/26/2022)**: [SAVi++: Towards End-to-End Object-Centric Learning from Real-World Videos](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/116%20SAVi%2B%2B%20Towards%20End-to-End%20Object-Centric%20Learning%20from%20Real-World%20Videos.pdf)
	
* **Day 117 (04/27/2022)**: [Disentangling visual and written concepts in CLIP](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/117%20Disentangling%20visual%20and%20written%20concepts%20in%20CLIP.pdf)
	
* **Day 118 (04/28/2022)**: [Action Spotting using Dense Detection Anchors Revisited Submission to the SoccerNet Challennge 2022](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/118%20Action%20Spotting%20using%20Dense%20Detection%20Anchors%20Revisited%20Submission%20to%20the%20SoccerNet%20Challennge%202022.pdf)
	
* **Day 119 (04/29/2022)**: [Improved surface reconstruction using high-frequency details](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/119%20Improved%20surface%20reconstruction%20using%20high-frequency%20details.pdf)
	
* **Day 120 (04/30/2022)**: [PeQuENet: Perceptual Quality Enhancement of Compressed Video with Adaptation- and Attentio-based Network](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/120%20PeQuENet%20Perceptual%20Quality%20Enhancement%20of%20Compressed%20Video%20with%20Adaptation-%20and%20Attentio-based%20Network.pdf)
	
* **Day 121 (05/01/2022)**: [Dual Contrastive Attributed Graph Clustering Network](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/121%20Dual%20Contrastive%20Attributed%20Graph%20Clustering%20Network.pdf)
	
* **Day 122 (05/02/2022)**: [Lifelong Wandering A realistic few-shot online continual learning setting](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/122%20Lifelong%20Wandering%20A%20realistic%20few-shot%20online%20continual%20learning%20setting.pdf)
	
* **Day 123 (05/03/2022)**: [Technical Report for Argoverse2 Challenge 2022 - Motion Forecasting Task](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/123%20Technical%20Report%20for%20Argoverse2%20Challenge%202022%20-%20Motion%20Forecasting%20Task.pdf)
	
* **Day 124 (05/04/2022)**: [Analysis and Extensions of Adversarial Training for Video Classification](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/124%20Analysis%20and%20Extensions%20of%20Adversarial%20Training%20for%20Video%20Classification.pdf)

* **Day 125 (05/05/2022)**: [A Simple Baseline for BEV Perception Without LiDAR](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/125%20A%20Simple%20Baseline%20for%20BEV%20Perception%20Without%20LiDAR.pdf)
	
* **Day 126 (05/06/2022)**: [DreamNet A Deep Riemannian Network based on SPD Manifold Learning for Visual Classification](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/126%20DreamNet%20A%20Deep%20Riemannian%20Network%20based%20on%20SPD%20Manifold%20Learning%20for%20Visual%20Classification.pdf)

* **Day 127 (05/07/2022)**: [Multi-scale Cooperative Multimodal Transformers for Multimodal Sentiment Analysis in Videos](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/127%20Multi-scale%20Cooperative%20Multimodal%20Transformers%20for%20Multimodal%20Sentiment%20Analysis%20in%20Videos.pdf)

* **Day 128 (05/08/2022)**: [Image Captioning based on Feature Refinement and Reflecting Decoding](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/128%20Image%20Captioning%20based%20on%20Feature%20Refinement%20and%20Reflecting%20Decoding.pdf)

* **Day 129 (05/09/2022)**: [Patch-level Representation Learning for Self-supervised Vision Transformers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/129%20Patch-level%20Representation%20Learning%20for%20Self-supervised%20Vision%20Transformers.pdf)

* **Day 130 (05/10/2022)**: [Joint Class-Affinity Loss Correction for Robust Medical Image Segmentation with Noisy Labels](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/130%20Joint%20Class-Affinity%20Loss%20Correction%20for%20Robust%20Medical%20Image%20Segmentation%20with%20Noisy%20Labels.pdf)

* **Day 131 (05/11/2022)**: [Balancing Discriminability and Transferability for Source-Free Domain Adaptation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/131%20Balancing%20Discriminability%20and%20Transferability%20for%20Source-Free%20Domain%20Adaptation.pdf)

* **Day 132 (05/12/2022)**: [Backbones-Review Feature Extraction Networks for Deep Learning and Deep RL Approaches](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/132%20Backbones-Review%20Feature%20Extraction%20Networks%20for%20Deep%20Learning%20and%20Deep%20RL%20Approaches.pdf)

* **Day 133 (05/13/2022)**: [DeepFormableTag End-to-end Generation and Recognition of Deformable Fiducial Markers](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/133%20DeepFormableTag%20End-to-end%20Generation%20and%20Recognition%20of%20Deformable%20Fiducial%20Markers.pdf)

* **Day 134 (05/14/2022)**: [CARLANE: A Lane Detection Benchmark for Unsupervised Domain Adaptation from Simulation to multiple Real-World Domains](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/134%20CARLANE%20A%20Lane%20Detection%20Benchmark%20for%20Unsupervised%20Domain%20Adaptation%20from%20Simulation%20to%20multiple%20Real-World%20Domains.pdf)
	
* **Day 135 (05/15/2022)**: [An Improved Normed-Deformable Convolution for Crowd Counting](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/135%20An%20Improved%20Normed-Deformable%20Convolution%20for%20Crowd%20Counting.pdf)
	
* **Day 136 (05/16/2022)**: [A Simple Baseline for Adversarial Domain Adaptation-based Unsupervised Flood Forecasting](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/136%20A%20Simple%20Baseline%20for%20Adversarial%20Domain%20Adaptation-based%20Unsupervised%20Flood%20Forecasting.pdf)
	
* **Day 137 (05/17/2022)**: [Channel Importance Matters in Few-Shot Image Classification](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/137%20Channel%20Importance%20Matters%20in%20Few-Shot%20Image%20Classification.pdf)
	
* **Day 138 (05/18/2022)**: [Trajectory-guided Control Prediction for End-to-end Autonomous Driving A Simple yet Strong Baseline](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/138%20Trajectory-guided%20Control%20Prediction%20for%20End-to-end%20Autonomous%20Driving%20A%20Simple%20yet%20Strong%20Baseline.pdf)
	
* **Day 139 (05/19/2022)**: [Self-Adaptive Label Augmentation for Semi-supervised Few-shot Classification](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/139%20Self-Adaptive%20Label%20Augmentation%20for%20Semi-supervised%20Few-shot%20Classification.pdf)
	
* **Day 140 (05/20/2022)**: [Zero-Shot Video Question Answering via Frozen Bidirectional Language Models](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/140%20Zero-Shot%20Video%20Question%20Answering%20via%20Frozen%20Bidirectional%20Language%20Models.pdf)
	
* **Day 141 (05/21/2022)**: [Volumetric Supervised Contrastive Learning for Seismic Semantic Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/141%20Volumetric%20Supervised%20Contrastive%20Learning%20for%20Seismic%20Semantic%20Segmentation.pdf)
	
* **Day 142 (05/22/2022)**: [K-Radar 4D Radar Object Detection Dataset and Benchmark for Autonomous Driving in Various Weather Conditions](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/142%20K-Radar%204D%20Radar%20Object%20Detection%20Dataset%20and%20Benchmark%20for%20Autonomous%20Driving%20in%20Various%20Weather%20Conditions.pdf)
	
* **Day 143 (05/23/2022)**: [RefCrowd: Grounding the Target in Crowd with Referring Expressions](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/143%20RefCrowd%20Grounding%20the%20Target%20in%20Crowd%20with%20Referring%20Expressions.pdf)
	
* **Day 144 (05/24/2022)**: [Level 2 Autonomous Driving on a Single Device Driving into the Devils of OpenPilot](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/144%20Level%202%20Autonomous%20Driving%20on%20a%20Single%20Device%20Driving%20into%20the%20Devils%20of%20OpenPilot.pdf)
	
* **Day 145 (05/25/2022)**: [Nucleus Segmentation and Analysis in Breast Cancer with the MIScnn Framework](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/145%20Nucleus%20Segmentation%20and%20Analysis%20in%20Breast%20Cancer%20with%20the%20MIScnn%20Framework.pdf)
	
* **Day 146 (05/26/2022)**: [Asymptotic Soft Cluster Pruning for Deep Neural Networks](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/146%20Asymptotic%20Soft%20Cluster%20Pruning%20for%20Deep%20Neural%20Networks.pdf)
	
* **Day 147 (05/27/2022)**: [Online Segmentation of LiDAR Sequences Dataset and Algorithm](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/147%20Online%20Segmentation%20of%20LiDAR%20Sequences%20Dataset%20and%20Algorithm.pdf)
	
* **Day 148 (05/28/2022)**: [Selective Multi-Scale Learning for Object Detection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/148%20Selective%20Multi-Scale%20Learning%20for%20Object%20Detection.pdf)
	
* **Day 149 (05/29/2022)**: [HaGRID: Hand Gesture Recognition Image Dataset](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/149%20HaGRID%20-%20Hand%20Gesture%20Recognition%20Image%20Dataset.pdf)
	
* **Day 150 (05/30/2022)**: [Adapting Self-Supervised Vision Transformers by Probing Attention-Conditioned Masking Consistency](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/150%20Adapting%20Self-Supervised%20Vision%20Transformers%20by%20Probing%20Attention-Conditioned%20Masking%20Consistency.pdf)
	
* **Day 151 (05/31/2022)**: [Multi-scale Feature Extraction and Fusion for Online Knowledge Distillation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/151%20Multi-scale%20Feature%20Extraction%20and%20Fusion%20for%20Online%20Knowledge%20Distillation.pdf)
	
* **Day 152 (06/01/2022)**: [Delving into the Scale Variance Problem in Object Detection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/152%20Delving%20into%20the%20Scale%20Variance%20Problem%20in%20Object%20Detection.pdf)
	
* **Day 153 (06/02/2022)**: [Open-Set Representation with Gradient-based Representations](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/153%20Open-Set%20Representation%20with%20Gradient-based%20Representations.pdf)
	
* **Day 154 (06/03/2022)**: [Simple and Efficient Architectures for Semantic Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/154%20Simple%20and%20Efficient%20Architectures%20for%20Semantic%20Segmentation.pdf)
	
* **Day 155 (06/04/2022)**: [Rank the triplets A ranking-based multiple instance learning framework for detecting HPV infection in head and neck cancers using routine H&E images](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/155%20Rank%20the%20triplets%20A%20ranking-based%20multiple%20instance%20learning%20framework%20for%20detecting%20HPV%20infection%20in%20head%20and%20neck%20cancers%20using%20routine%20H%26E%20images.pdf)

* **Day 156 (06/05/2022)**: [Adversarial Patch Attacks and Defences in Vision-based Tasks A Survey](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/156%20Adversarial%20Patch%20Attacks%20and%20Defences%20in%20Vision-based%20Tasks%20A%20Survey.pdf)

* **Day 157 (06/06/2022)**: [iBoot: Image-bootstrapped Self-Supervised Video Representation Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/157%20iBoot%20Image-bootstrapped%20Self-Supervised%20Video%20Representation%20Learning.pdf)

* **Day 158 (06/07/2022)**: [Realistic One-Shot Mesh-based Head Avatars](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/158%20Realistic%20One-shot%20Mesh-based%20Head%20Avatars.pdf)
	
* **Day 159 (06/08/2022)**: [Real-World Single Image Super-Resolution Under Rainy Condition](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/159%20Real-World%20Single%20Image%20Super-Resolution%20Under%20Rainy%20Condition.pdf)
	
* **Day 160 (06/09/2022)**: [Beyond Supervised v/s Unsupervised: Representative Benchmarking and Analysis of Image Representation Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/160%20Beyond%20Supervised%20vs%20Unsupervised%20Representative%20Benchmarking%20and%20Analysis%20of%20Image%20Representation%20Learning.pdf)
	
* **Day 161 (06/10/2022)**: [OmniMAE: Single Model Masked Pretraining on Images and Videos](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/161%20OmniMAE%20Single%20Model%20Masked%20Pretraining%20on%20Images%20and%20Videos.pdf)
	
* **Day 162 (06/11/2022)**: [Spatially-Adaptive Multilayer Selection for GAN Inversion and Editing](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/162%20Spatially-Adaptive%20Multilayer%20Selection%20for%20GAN%20Inversion%20and%20Editing.pdf) 

* **Day 163 (06/12/2022)**: [MixGen: A New Multi-Modal Data Augmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/163%20MixGen%20A%20New%20Multi-Modal%20Data%20Augmentation.pdf)
	
* **Day 164 (06/13/2022)**: [Controllable 3D Face Synthesis with Conditional Generative Occupancy Fields](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/164%20Controllable%203D%20Face%20Synthesis%20with%20Conditional%20Generative%20Occupancy%20Fields.pdf)
	
* **Day 165 (06/14/2022)**: [Unified Fourier-based Kernel and Nonlinearity Design for Equivariant Networks on Homogeneous Spaces](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/165%20Unified%20Fourier-based%20Kernel%20and%20Nonlinearity%20Design%20for%20Equivariant%20Networks%20on%20Homogeneous%20Spaces.pdf)
	
* **Day 166 (06/15/2022)**: [Virtual Correspondence: Humans as a Cue for Extreme-View Geometry](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/166%20Virtual%20Correspondence%20Humans%20as%20a%20Cue%20for%20Extreme-View%20Geometry.pdf)
	
* **Day 167 (06/16/2022)**: [SHIFT: A Synthetic Driving Dataset for Continuous Multi-Task Domain Adaptation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/167%20SHIFT%20A%20Synthetic%20Driving%20Dataset%20for%20Continuous%20Multi-Task%20Domain%20Adaptation.pdf)
	
* **Day 168 (06/17/2022)**: [Unbiased 4D Monocular 4D Reconstruction with a Neural Deformable Model](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/168%20Unbiased%204D%20Monocular%204D%20Reconstruction%20with%20a%20Neural%20Deformation%20Model.pdf)
	
* **Day 169 (06/18/2022)**: [Towards Robust Blind Restoration with Codebook Lookup Transformer](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/169%20Towards%20Robust%20Blind%20Face%20Restoration%20with%20Codebook%20Lookup%20Transformer.pdf)
	
* **Day 170 (06/19/2022)**: [A High Resolution Multi-exposure Stereoscopic Image & Video Database of Natural Scenes](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/170%20A%20High%20Resolution%20Multi-exposure%20Stereoscopic%20Image%20%26%20Video%20Database%20of%20Natural%20Scenes.pdf)
	
* **Day 171 (06/20/2022)**: [Surgical-VQA: Visual Question Answering in Surgical Scenes using Transformer](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/171%20Surgical-VQA%20Visual%20Question%20Answering%20in%20Surgical%20Scenes%20using%20Transformer.pdf)
	
* **Day 172 (06/21/2022)**: [AdvSmo: Black-box Adversarial Attack by Smoothing Linear Structure of Texture](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/172%20AdvSmo%20Black-box%20Adversarial%20Attack%20by%20Smoothing%20Linear%20Structure%20of%20Texture.pdf)
	
* **Day 173 (06/22/2022)**: [SpA-Former: Transformer image shadow detection and removal via spatial attention](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/173%20SpA-Former%20Transformer%20image%20shadow%20detection%20and%20removal%20via%20spatial%20attention.pdf)
	
* **Day 174 (06/23/2022)**: [Specialize and Fuse: Pyramidal Output Representation for Semantic Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/174%20Specialize%20and%20Fuse%20Pyramidal%20Output%20Representation%20for%20Semantic%20Segmentation.pdf)
	
* **Day 175 (06/24/2022)**: [3D Morphable Face Models - Past, Present, and  Future](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/175%203D%20Morphable%20Face%20Models%20-%20Past%2C%20Present%2C%20and%20Future.pdf)

* **Day 176 (06/24/2022)**: [Semantic Abstraction Open-World 3D Scene Understanding from 2D Vision-Language Models](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/176%20Semantic%20Abstraction%20Open-World%203D%20Scene%20Understanding%20from%202D%20Vision-Language%20Models.pdf)

* **Day 177 (06/26/2022)**: [TinyCD: A (Not So) Deep Learning Model for Change Detection](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/177%20TinyCD%20A%20(Not%20So)%20Deep%20Learning%20Model%20for%20Change%20Detection.pdf)

* **Day 178 (06/27/2022)**: [Low-Complexity Approximate Convolutional Neural Network](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/178%20Low-complexity%20Approximate%20Convolutional%20Neural%20Networks.pdf)
	
* **Day 179 (06/28/2022)**: [Robust Trajectory Prediction Against Adversarial Attacks](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/179%20Robust%20Trajectory%20Prediction%20against%20Adversarial%20Attacks.pdf)

* **Day 180 (06/29/2022)**: [A review of Deep Learning Techniques for COVID-19 Identification on Chest CT Images](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/180%20A%20review%20of%20Deep%20learning%20Techniques%20for%20COVID-19%20identification%20on%20Chest%20CT%20images.pdf)

* **Day 181 (06/30/2022)**: [A Multi-stage Framwork with Mean Subspace Computation and Recursive Feedbackk for Online Unsupervised Domain Adaptation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/181%20A%20Multi-stage%20Framework%20with%20Mean%20Subspace%20Computation%20and%20Recursive%20Feedback%20for%20Online%20Unsupervised%20Domain%20Adaptation.pdf)

* **Day 182 (07/01/2022)**: [MulViMOtion: Shape-aware 3D Mycordial Motion Tracking from Multi-View Cardiac MRI](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/182%20MulViMotion%20Shape-aware%203D%20Myocardial%20Motion%20Tracking%20from%20Multi-View%20Cardiac%20MRI.pdf)
	
* **Day 183 (07/02/2022)**: [Resolution enhanced of placenta histological images using Deep Learning](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/183%20Resolution%20enhancement%20of%20placenta%20histological%20images%20using%20Deep%20Learning.pdf)
	
* **Day 184 (07/03/2022)**: [Temporal Extrapolation of heart wall segmentation in cardiac magnetic resonance images via pixel tracking](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/184%20Temporal%20extrapolation%20of%20heart%20wall%20segmentation%20in%20cardiac%20magnetic%20resonance%20images%20via%20pixel%20tracking.pdf)
	
* **Day 185 (07/04/2022)**: [LRIP-Net: Low Resolution Image Prior based Network  for Limited-Angle CT Reconstruction](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/185%20LRIP-Net%20Low-Resolution%20Image%20Prior%20based%20Network%20for%20Limited-Angle%20CT%20Reconstruction.pdf)
	
* **Day 186 (07/05/2022)**: [MultiEarth 2022 - The Champion Solution for Image-](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/186%20MultiEarth%202022%20-%20The%20Champion%20Solution%20for%20Image-to-Image%20Translation%20Challenge%20via%20Generation%20Models.pdf)
	
* **Day 187 (07/06/2022)**: [Speckle2Speckle: Unsupervised Learning of Ultrasound Speckle Filtering w/o Clean Data](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/187%20Speckle2Speckle%20Unsupervised%20Learning%20of%20Ultrasound%20Speckle%20Filtering%20wo%20Clean%20Data.pdf)
	
* **Day 188 (07/07/2022)**: [DA2 Dataset: Towards Dexterity-Aware Dual-Arm Grasping](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/188%20DA2%20Dataset%20Towards%20Dexterity-Aware%20Dual-Arm%20Grasping.pdf)

* **Day 189 (07/08/2022)**: [Feather-Light Fourier Domain Adaptation in Magnetic Resonance Imaging](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/189%20Feather-Light%20Fourier%20Domain%20Adaptation%20in%20Magnetic%20Resonance%20Imaging.pdf)

* **Day 190 (07/09/2022)**: [One Object at a Time: Accurate and Structure from Motion for Robots](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/190%20One%20Object%20at%20a%20Time%20Accurate%20and%20Structure%20From%20Motion%20for%20Robots.pdf)
	
* **Day 191 (07/10/2022)**: [An Enhanced Deep Learning Technique for Prostate Cancer Identification based on MRI Scans](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/191%20An%20Enhanced%20Deep%20Learning%20Technique%20for%20Prostate%20Cancre%20Identification%20based%20on%20MRI%20Scans.pdf)
	
* **Day 192 (07/11/2022)**: [XOOD: Extreme Value Based Out-Of-Distribution Detection for Image Classification](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/192%20XOOD%20Extreme%20Value%20Based%20Out-Of-Distribution%20Detection%20for%20Image%20Classification.pdf)
	
* **Day 193 (07/12/2022)**: [Lung Nodules segmentation from CT with DeepHealth Toolkit](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/193%20Lung%20nodules%20segmentation%20from%20CT%20with%20DeepHealth%20Toolkit.pdf)
	
* **Day 194 (07/13/2022)**: [UniToBrain dataset: a Brain Perfusion Dataset](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/194%20UniToBrain%20dataset%20a%20Brain%20Perfusion%20Dataset.pdf)
	
* **Day 195 (07/14/2022)**: [TransDeepLab: Convolution-Free Transformer-based DeepLab v3+ for Medical Image Segmentation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/195%20TransDeepLab%20Convolution-Free%20Transformer-based%20DeepLab%20v3%2B%20for%20Medical%20Image%20Segmentation.pdf)
	
* **Day 196 (07/15/2022)**: [Interaction Mix and Match: Synthesizing Close Interaction using Conditional Hierarchical GAN with Multi-Hot Class Embedding](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/196%20Interaction%20Mix%20and%20Match%20Synthesizing%20Close%20Interaction%20using%20Conditional%20Hierarchical%20GAN%20with%20Multi-Hot%20Class%20Embedding.pdf)
	
* **Day 197 (07/16/2022)**: [Dynamic Batch Adaptation](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/197%20Dynamic%20Batch%20Adaptation.pdf)
	
* **Day 198 (07/17/2022)**: [Attacking Adversarial Defenses by Smoothing the Loss Landscape](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/198%20Attacking%20Adversarial%20Defences%20by%20Smoothing%20the%20Loss%20Landscape.pdf)
	
* **Day 199 (07/18/2022)**: [VolTeMorph: Realtime, Controllable and Generalizable Animation of Volumetric Representations](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/199%20VolTeMorph%20Realtime%2C%20Controllable%20and%20Generalisable%20Animation%20of%20Volumetric%20Representations.pdf)
	
* **Day 200 (07/19/2022)**: [Fast Two-Step Blind Optical Aberration Correction](https://github.com/AnshMittal1811/100_Days_for_ComputerVision_Papers/blob/master/200%20Fast%20Two-step%20Blind%20Optical%20Aberration%20Correction.pdf)	

* **Day 201 (07/20/2022)**: []()

* **Day 202 (07/21/2022)**: []()

* **Day 203 (07/22/2022)**: []()

* **Day 204 (07/23/2022)**: []()

* **Day 205 (07/24/2022)**: []()

* **Day 206 (07/25/2022)**: []()

* **Day 207 (07/26/2022)**: []()

* **Day 208 (07/27/2022)**: []()

* **Day 209 (07/28/2022)**: []()
  
* **Day 210 (07/29/2022)**: []()

* **Day 211 (07/30/2022)**: []()

* **Day 212 (07/31/2022)**: []()

* **Day 213 (08/01/2022)**: []()

* **Day 214 (08/02/2022)**: []()

* **Day 215 (08/03/2022)**: []()

* **Day 216 (08/04/2022)**: []()

* **Day 217 (08/05/2022)**: []()

* **Day 218 (08/06/2022)**: []()

* **Day 219 (08/07/2022)**: []()

* **Day 220 (08/08/2022)**: []()

* **Day 221 (08/09/2022)**: []()

* **Day 222 (08/10/2022)**: []()

* **Day 223 (08/11/2022)**: []()

* **Day 224 (08/12/2022)**: []()

* **Day 225 (08/13/2022)**: []()

* **Day 226 (08/14/2022)**: []()

* **Day 227 (08/15/2022)**: []()

* **Day 228 (08/16/2022)**: []()

* **Day 229 (08/17/2022)**: []()

* **Day 230 (08/18/2022)**: []()
	
* **Day 231 (08/19/2022)**: []()

* **Day 232 (08/20/2022)**: []()

* **Day 233 (08/21/2022)**: []()

* **Day 234 (08/22/2022)**: []()
	
* **Day 235 (08/23/2022)**: []()
	
* **Day 236 (08/24/2022)**: []()
	
* **Day 237 (08/25/2022)**: []()
	
* **Day 238 (08/26/2022)**: []()
	
* **Day 239 (08/27/2022)**: []()
	
* **Day 240 (08/28/2022)**: []()
	
* **Day 241 (08/29/2022)**: []()
	
* **Day 242 (08/30/2022)**: []()
	
* **Day 243 (08/31/2022)**: []()
	
* **Day 244 (09/01/2022)**: []()
	
* **Day 245 (09/02/2022)**: []()
	
* **Day 246 (09/03/2022)**: []()
	
* **Day 247 (09/04/2022)**: []()
	
* **Day 248 (09/05/2022)**: []()
	
* **Day 249 (09/06/2022)**: []()
	
* **Day 250 (09/07/2022)**: []()
	
* **Day 251 (09/08/2022)**: []()
	
* **Day 252 (09/09/2022)**: []()
	
* **Day 253 (09/10/2022)**: []()
	
* **Day 254 (09/11/2022)**: []()

* **Day 255 (09/12/2022)**: []()
	
* **Day 256 (09/13/2022)**: []()
	
* **Day 257 (09/14/2022)**: []()
	
* **Day 258 (09/15/2022)**: []()
	
* **Day 259 (09/16/2022)**: []()
	
* **Day 260 (09/17/2022)**: []()
