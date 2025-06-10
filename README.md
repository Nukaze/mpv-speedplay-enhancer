# MPV Speedplay Enhancer

A high-performance video player, portable build of MPV for Windows x64 that delivers hardware-accelerated video playback, modern GPU output and ultra-fast seeking. Perfect for playing long videos at high speeds (e.g., x100) without lag. No installation required - just unzip and run.

### 🎯 Key Features

- 📦 **Portable** - No installation required
- ⏩ **High-Speed** - Optimized for x100+ playback
- ⚡ **Smooth** - Frame interpolation for fluid motion
- 🔍 **Fast** - Ultra-quick seeking and loading
- 🚀 **Efficient** - Hardware-accelerated decoding
- 🎮 **Modern** - Vulkan/D3D11 GPU output
- 🎨 **Accurate** - Color-managed output

___

## 📥 Quick Start

### Method 1: Using the Extracted Folder
1. Navigate to the extracted folder `mpv-speedplay-enhancer-2025-06-10-x86_64`
2. Run `mpv.exe` directly or set as default video player app

### Method 2: Using the ZIP Archive
1. Download `mpv-speedplay-enhancer-2025-06-10-x86_64.zip`
2. Extract to your desired directory
3. Do the same as **Method 1**

___

## ⚙️ System Requirements

### 🖥️ Minimum Specs
- **CPU**: Intel Core i5 / AMD Ryzen 5 or better
- **GPU**: NVIDIA GTX 1050 Ti / AMD RX 560 or better
- **RAM**: 8 GB minimum
- **OS**: Windows 10/11 64-bit

### 💪 Recommended Specs
For optimal performance, especially at high playback speeds:

- **CPU**: Intel Core i7/i9 or AMD Ryzen 7/9
- **GPU**: NVIDIA RTX 2060 or better / AMD RX 5600 XT or better
- **RAM**: 16 GB or more
- **Storage**: SSD recommended for faster seeking

___

## ⚠️ Performance Tuning Notes

If you experience performance issues, try these optimizations:

1. **Disable Frame Interpolation**
   - Edit `mpv.conf` and set `interpolation=no`
   - This significantly reduces CPU/GPU load
   - Note: Frame interpolation (`interpolation=yes`) significantly increases CPU/GPU usage; disable on low-end hardware

2. **Use Alternative Video Output**
   - If `vo=gpu-next` causes issues, switch to `vo=opengl`
   - Add `vo=opengl` to `mpv.conf`
   - Note: Modern GPU output (`vo=gpu-next`) may not be supported on older GPUs

3. **Adjust Hardware Decoding**
   - For NVIDIA: `hwdec=nvdec`
   - For AMD: `hwdec=amf`
   - For Intel: `hwdec=d3d11va`

4. **Memory Management**
   - Reduce cache size: `cache=yes cache-secs=30`
   - Limit demuxer cache: `demuxer-max-bytes=500M`

5. **High-Speed Playback Tips**
   - High-speed playback (x100+) requires sufficient CPU/GPU resources
   - Consider reducing playback speed if system struggles
   - Use hardware decoding for better performance

___

## 📝 License

This project is licensed under the GNU General Public License v2.0 (GPL-2.0). See the [LICENSE](LICENSE) file for details.

The GPL-2.0 is a free software license that guarantees end users the freedom to run, study, share, and modify the software. For more information about the GPL-2.0, visit [https://www.gnu.org/licenses/gpl-2.0.html](https://www.gnu.org/licenses/gpl-2.0.html).
