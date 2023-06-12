# 3D human pose estimation in video with temporal convolutions and semi-supervised training

Based on the success of 2d human pose estimation, it directly "lifts" a sequence of 2d keypoints to 3d keypoints.

## Results and Models

### Human3.6m Dataset

| Arch                                                    | Receptive Field | MPJPE | P-MPJPE | N-MPJPE |                           ckpt                           |                           log                           |
| :------------------------------------------------------ | :-------------: | :---: | :-----: | :-----: | :------------------------------------------------------: | :-----------------------------------------------------: |
| [VideoPose3D-supervised](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-27frm-supv_8xb128-80e_h36m.py) |       27        | 40.1  |  30.1   |    /    | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_27frames_fullconv_supervised-fe8fbba9_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_27frames_fullconv_supervised_20210527.log.json) |
| [VideoPose3D-supervised](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-81frm-supv_8xb128-80e_h36m.py) |       81        | 39.1  |  29.3   |    /    | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_81frames_fullconv_supervised-1f2d1104_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_81frames_fullconv_supervised_20210527.log.json) |
| [VideoPose3D-supervised](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-243frm-supv_8xb128-80e_h36m.py) |       243       |       |         |    /    | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_243frames_fullconv_supervised-880bea25_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_243frames_fullconv_supervised_20210527.log.json) |
| [VideoPose3D-supervised-CPN](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-1frm-supv-cpn-ft_8xb128-80e_h36m.py) |        1        | 53.0  |  41.3   |    /    | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_1frame_fullconv_supervised_cpn_ft-5c3afaed_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_1frame_fullconv_supervised_cpn_ft_20210527.log.json) |
| [VideoPose3D-supervised-CPN](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-243frm-supv-cpn-ft_8xb128-200e_h36m.py) |       243       |       |         |    /    | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_243frames_fullconv_supervised_cpn_ft-88f5abbb_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_243frames_fullconv_supervised_cpn_ft_20210527.log.json) |
| [VideoPose3D-semi-supervised](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-27frm-semi-supv_8xb64-200e_h36m.py) |       27        | 57.2  |  42.4   |  54.2   | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_27frames_fullconv_semi-supervised-54aef83b_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_27frames_fullconv_semi-supervised_20210527.log.json) |
| [VideoPose3D-semi-supervised-CPN](/configs/body_3d_keypoint/video_pose_lift/h36m/vid-pl_videopose3d-27frm-semi-supv-cpn-ft_8xb64-200e_h36m.py) |       27        | 67.3  |  50.4   |  63.6   | [ckpt](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_27frames_fullconv_semi-supervised_cpn_ft-71be9cde_20210527.pth) | [log](https://download.openmmlab.com/mmpose/body3d/videopose/videopose_h36m_27frames_fullconv_semi-supervised_cpn_ft_20210527.log.json) |