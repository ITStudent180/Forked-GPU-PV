# GPU-PV Fork - Read Me

### Key Changes:
- **Removed Parsec references**: Looking for alternatives? Try the following:
  - **Moonlight**
  - **Sunshine**
  - **AMD Link**
  - **Steam Remote Play**
  
- **Script not running?**  
  Ensure **Powershell script execution** is enabled by running the following command in an elevated PowerShell session (Run as Administrator):

  ```powershell
  Set-ExecutionPolicy RemoteSigned
  ```

  This command allows scripts downloaded from the internet to run if they are signed by a trusted publisher, while still allowing local scripts to run without a signature.

- **Resource Enhancements**:  
  Increased provisioning for:
  - Disk space
  - GPU resources
  - CPU cores

- **User-Friendly Comments**:  
  Added more descriptive comments throughout the script to improve usability.

---

## How to Enable Checkpoints in Hyper-V

1. **Power off the Guest VM**.
2. Open the VM settings inside Hyper-V Manager.
3. Navigate to the **Checkpoints** section.
4. Choose between:
   - **Production Checkpoints** (Recommended)
   - **Standard Checkpoints**

### Production Checkpoints (Recommended):
- These are filesystem snapshots of your virtual disk.
- Microsoft defines production checkpoints as "point-in-time" images of a virtual machine that can be restored later. 
- They use backup technology inside the guest operating system, making them fully supported for production workloads.

### Standard Checkpoints:
- Capture the state, data, and hardware configuration of a running virtual machine.
- Primarily used for development and testing scenarios.
- Useful for recreating specific states or conditions of a VM to troubleshoot problems.
