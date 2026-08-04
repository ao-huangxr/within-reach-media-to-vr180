# Within Reach Flat Media VR180 0.1.0 Beta 2 (macOS Build 4)

## 中文

- 修复大视频导入时界面长时间无响应；
- Production Planning 已移至后台；
- Mono 和 SBS 视频使用持续 ROI Renderer；
- SBS H.265 不再生成逐帧 PNG；
- 视频透明 MOV 使用持续流式 QTRLE；
- 动态 QTRLE 启用 `g=300` 时间压缩；
- 改进进度、取消和 FFmpeg/FFprobe 子进程清理；
- 降低动态视频导出的临时磁盘和内存压力；
- 保持精确 50、60000/1001（59.94）和 60 fps 合同。

### 已知限制

- 透明 MOV 为 QuickTime Animation/QTRLE，建议用于约 5–10 秒的短透明素材；
- 长时真实摄影透明 MOV 仍可能非常大；106.573 秒压力实验约为 24.768 GiB；
- HEVC with Alpha 不包含在本版本；
- 当前 M1 Pro 环境无法建立 VideoToolbox HEVC 编码器，普通 H.265 会使用已捆绑的受支持编码路径；
- 不承诺长透明视频实时播放。

## English

- Fixes prolonged UI unresponsiveness while importing large video files;
- Moves Production Planning to a background worker;
- Uses continuous ROI rendering for Mono and SBS video;
- Removes per-frame PNG generation from SBS H.265 export;
- Streams transparent video directly to QuickTime Animation/QTRLE MOV;
- Enables `g=300` temporal compression for dynamic QTRLE;
- Improves progress reporting, cancellation, and FFmpeg/FFprobe cleanup;
- Reduces temporary-disk and memory pressure for dynamic video export;
- Preserves exact 50, 60000/1001 (59.94), and 60 fps contracts.

### Known limitations

- Transparent MOV uses QuickTime Animation/QTRLE and is recommended for short transparent clips of about 5–10 seconds;
- Long photographic transparent MOV files may still be extremely large; a 106.573-second stress test produced about 24.768 GiB;
- HEVC with Alpha is not included in this release;
- The current M1 Pro environment cannot establish the VideoToolbox HEVC encoder; ordinary H.265 uses the bundled supported encoder path;
- Real-time playback of long transparent video is not guaranteed.
