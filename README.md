# 3D-Pose-and-Segmentation-for-AR-in-MIS
In this project, we present deep convolution neural network (DCNN) for simultaneously getting surgical instrument segmentation and geometric features for 3D pose estimation to solve the current ambiguities of AR based application in MIS. Additionally, we add detection sub-network to our SIMO-DCNN to get the tool flag. Tool flag will provide the constrain of estimating pose or not. The proposed network with different responsible sub-networks has been trained in an end-to-end fashion and each sub-network of the SIMO-DCNN has different loss functions to get responsible output.  We validate our proposed approach on both ex-vivo and in-vivo laparoscopic images where we are able to reach improved results over existing state-of-the-art approaches on the same dataset. The geometric features obtained from the proposed SIMO network are used to estimate the 3D pose of surgical instruments by geometric solver. <br>

The pictorial presentation of overall pipeline that has been accomplished is shown in above figure.  Firstly, input images are feed to CRB block which is a bunch of convolution  and relu activation  with  sub-sampling  and  is  shared  by  all  others  sub-networks for detection, segmentation and regression simultaneously.  FCS is the fully connected layer followed by the softmax classifier that provides the information about the tool presence in the image frame and termed as detection sub-network. If the detected tool flag is yes from the detection sub-network, the pose of the surgical tool will be estimated and vice-versa. DRBS named as segmentation sub-network and DRB named as regression sub-network are the bunch deconvolution for semantic tissue or instrument pixels labelling and the regression to get three geometric features for pose estimation respectively.  

#### Written by-
#### Md. Kamrul Hasan 
#### Erasmus Scholar on Medical Imaging and Application (MAIA) [http://maiamaster.udg.edu/]
#### For more details write me at kamruleeekuet@gmail.com

The idea for the single input multiple output (SIMO) DCNN along with transfer learning is shown in the Figure below. 
![simo](https://user-images.githubusercontent.com/32570071/52538979-7cd2e700-2d79-11e9-91ef-620780feb8bb.png)

For the details about this project will be added later. 
