# Chinese DLL Readme / `chinese.dll` 说明

## 中文

### 文件位置

请将 `chinese.dll` 放在以下目录：

`Polar\Si9000\Lang\`

本工程中的目标文件路径为：

`Polar\Si9000\Lang\chinese.dll`

### 这份 `chinese.dll` 改了什么

这份语言包基于官方 `english.dll` 制作，主要做了以下修改：

1. 将界面字符串资源翻译为简体中文。
2. 对机器翻译结果做了人工校对和二次修正。
3. 修正了图表、阻抗、表面粗糙度、FOI、过孔检查、导入导出等专业术语。
4. 将 DLL 元数据中的语言名称改为 `Chinese` / `Chinese.dll`。
5. 保留了原始 DLL 的导出函数、类型库和资源结构，未修改主程序 EXE。

说明：

- 这是语言资源 DLL，不是破解补丁，也不改计算核心。
- 一些专业缩写按原文保留，例如 `RLGC`、`Touchstone`、`NEXT`、`FEXT`、`TanD`、`Huray`。

### 如何放置

1. 保留原来的 `english.dll` 不动。
2. 将 `chinese.dll` 复制到 `Lang` 目录。
3. 确认目录中同时存在：

   - `english.dll`
   - `chinese.dll`

### 如何选择

通常在软件中按下面路径选择语言：

`Configuration` -> `Language Settings`

然后：

1. 在语言列表中选择 `Chinese`。
2. 确认后关闭软件。
3. 重新启动软件，使语言切换生效。

### 是否需要“导入”

不需要单独“导入”语言包。

这类语言 DLL 只需要放到 `Lang` 目录中，然后在软件的语言设置里选择即可。

### 如果没有看到中文选项

请依次检查：

1. `chinese.dll` 是否确实放在 `Polar\Si9000\Lang\` 中。
2. 文件名是否为小写 `chinese.dll`。
3. 软件是否已经完全退出并重新启动。
4. 当前应用版本是否与语言 DLL 版本匹配。

本 DLL 的版本信息为：

- `FileVersion`: `25.01.0001`
- `ProductVersion`: `25.01.0001`

如果软件提示：

`The Language Resource file version does not match the Application version.`

说明语言包版本和当前程序版本不一致，需要换成匹配版本。

### 额外说明

- 这份 DLL 已针对当前目录中的 Si9000 安装包做过校对。
- 如果后续还想继续优化术语，可以继续在此文件基础上迭代。

---

## English

### File Location

Place `chinese.dll` in:

`Polar\Si9000\Lang\`

In this workspace, the target file is:

`Polar\Si9000\Lang\chinese.dll`

### What Was Changed

This language DLL was built from the official `english.dll` and includes:

1. Translation of UI string resources into Simplified Chinese.
2. Manual review and cleanup after machine translation.
3. Terminology fixes for graphs, impedance, surface roughness, FOI, via checks, and import/export dialogs.
4. Updated DLL metadata to `Chinese` / `Chinese.dll`.
5. Preserved exports, typelib, and resource structure from the original DLL.

Notes:

- This is a language resource DLL only.
- It does not patch the EXE or modify the solver engine.
- Some technical acronyms intentionally remain in English, such as `RLGC`, `Touchstone`, `NEXT`, `FEXT`, `TanD`, and `Huray`.

### How to Place It

1. Keep the original `english.dll`.
2. Copy `chinese.dll` into the `Lang` folder.
3. Make sure both files exist:

   - `english.dll`
   - `chinese.dll`

### How to Select It

The usual path inside the application is:

`Configuration` -> `Language Settings`

Then:

1. Select `Chinese` from the language list.
2. Close the application.
3. Restart the application for the change to take effect.

### Do You Need to Import It?

No separate import step is required.

This type of language DLL only needs to be placed in the `Lang` folder and then selected from the language settings UI.

### If Chinese Does Not Appear

Check the following:

1. `chinese.dll` is in `Polar\Si9000\Lang\`.
2. The filename is exactly `chinese.dll`.
3. The application has been fully restarted.
4. The DLL version matches the application version.

This DLL currently reports:

- `FileVersion`: `25.01.0001`
- `ProductVersion`: `25.01.0001`

If the application shows:

`The Language Resource file version does not match the Application version.`

then the language DLL version does not match your installed application build.
