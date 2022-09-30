# BeamCalib
轨检梁标定程序。
## 使用方法
### 命令行
- 获取帮助
  ```shell
  beam_calibr.exe --help
  ```
- 标定前激光器
  ```shell
  beam_calibr.exe --in=G:\标定-前-20220830-142824\ --out=config_front.yaml --ruler-width=1395 --meas-offset=295 --right-inner=2 --left-inner=0 --right-inner-offset=565,-71,268.5 --left-inner-offset=-565,-71,268.5 --inverse=true
  ```
- 标定后激光器
  ```shell
  beam_calibr.exe --in=G:\标定-后-20220830-143653 --out=config_back.yaml --ruler-width=1395 --meas-offset=295 --right-inner=1 --left-inner=3 --right-inner-offset=565,-71,-268.5 --left-inner-offset=-565,-71,-268.5
  ```
### 图形界面
  ```shell
  beam_calibr_gui.exe
  ```

（有 gif 演示，需要等待一会↓）

![](README.assets/demo.gif)

## What's Changed
* 消除 VTK deprecated warning 弹窗。 by @delyex in https://github.com/rail-check/BeamCalib/pull/6


**Full Changelog**: https://github.com/rail-check/BeamCalib/compare/v1.2...v1.3
