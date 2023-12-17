#How to enable checkpoints?
Poweroff Guest VM, go to vm settings inside hyper v > Checkpoints option enable Production or Standard Checkpoints. 
Production checkpoints are filesystem snapshots of your virtual disk. Easiest and Recommended option.

Microsoft Definitions:
Production checkpoints are "point in time" images of a virtual machine, which can be restored later on in a way that is completely supported for all production workloads. This is achieved by using backup technology inside the guest to create the checkpoint, instead of using saved state technology.

Standard checkpoints capture the state, data, and hardware configuration of a running virtual machine and are intended for use in development and test scenarios. Standard checkpoints can be useful if you need to recreate a specific state or condition of a running virtual machine so that you can troubleshoot a problem.


