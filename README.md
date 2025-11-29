# SBS Creator - Substance Designer 批量生成器
# SBS Creator - Substance Designer Batch Generator

一款强大的 GUI 工具，用于从贴图集合自动生成 Substance Designer (.sbs) 文件。该工具通过自动检测和链接贴图，简化了创建材质图表的工作流程。

A powerful GUI tool for automatically generating Substance Designer (.sbs) files from texture sets. This tool simplifies the workflow of creating material graphs by automatically detecting and linking texture maps.

**作者 / Author**: Mengshengyu + Claude sonnet 4.5

---

## 功能特点
## Features

- **批量处理**: 从材质文件夹目录批量生成多个 .sbs 文件
- **Batch Processing**: Generate multiple .sbs files from a directory of material folders

- **自动贴图识别**: 通过文件名关键词智能识别贴图类型（BaseColor、Normal、Roughness、AO 等）
- **Automatic Texture Detection**: Intelligently identifies texture types (BaseColor, Normal, Roughness, AO, etc.) by filename keywords

- **可自定义关键词**: 完全可自定义的关键词匹配系统，适应不同的命名规范
- **Customizable Keywords**: Fully customizable keyword matching system for different naming conventions

- **拖放支持**: 只需拖放任意贴图文件或文件夹即可自动检测材质目录
- **Drag & Drop Support**: Simply drag any texture file or folder to auto-detect the material directory

- **双语界面**: 支持英文和中文
- **Bilingual Interface**: Supports both English and Chinese

- **覆盖保护**: 自动跳过已存在文件或根据需要覆盖
- **Overwrite Protection**: Automatically skips existing files or overwrites them as needed

---

## 系统要求
## System Requirements

- Windows 10/11
- 无需额外软件（独立可执行文件）
- No additional software required (standalone executable)

---

## 使用方法
## How to Use

1. **启动应用程序**: 运行 `SBS Creator.exe`
   - **Launch the Application**: Run `SBS Creator.exe`

2. **选择材质目录**:
   - **Select Material Directory**:
   - 点击"选择目录"按钮，或
   - Click "Select Directory" button, OR
   - 将任意贴图文件或材质文件夹拖放到拖放区域
   - Drag and drop any texture file or material folder into the drop area
   - 工具会自动检测包含材质文件夹的根目录
   - The tool will automatically detect the root directory containing material folders

3. **自定义关键词（可选）**:
   - **Customize Keywords (Optional)**:
   - 在"关键字配置"部分调整贴图识别关键词
   - Adjust texture recognition keywords in the "Keyword Configuration" section
   - 关键词用逗号分隔（例如："basecolor, base_color, albedo"）
   - Keywords are comma-separated (e.g., "basecolor, base_color, albedo")
   - 每种贴图类型可以有多个关键词，实现灵活匹配
   - Each texture type can have multiple keywords for flexible matching

4. **生成 SBS 文件**:
   - **Generate SBS Files**:
   - 点击"全部生成"按钮
   - Click "Generate All" button
   - 工具将处理所选目录中的所有材质文件夹
   - The tool will process all material folders in the selected directory
   - 生成的 .sbs 文件将保存在同一目录中
   - Generated .sbs files will be saved in the same directory

5. **在 Substance Designer 中打开**:
   - **Open in Substance Designer**:
   - 在 Substance Designer 中打开任何生成的 .sbs 文件
   - Open any generated .sbs file in Substance Designer
   - 所有贴图将自动链接并可以使用
   - All textures will be automatically linked and ready to use

---

## 支持的贴图类型
## Supported Texture Types

- BaseColor / Albedo / Diffuse
- Normal
- Roughness
- Metallic
- Height / Displacement
- Ambient Occlusion (AO)
- Specular
- Glossiness
- Opacity

---

## 技术细节
## Technical Details

- **输出格式**: Substance Designer .sbs 格式（版本 1.1.0.202401）
- **Output Format**: Substance Designer .sbs format (version 1.1.0.202401)

- **贴图分辨率**: 2048x2048（SD 单位为 11x11）
- **Texture Resolution**: 2048x2048 (11x11 in SD units)

- **开发工具**: Python 3, PySide6 (Qt)
- **Built with**: Python 3, PySide6 (Qt)

---

## 语言支持
## Language Support

- 中文（简体）
- 中文 (Simplified Chinese)
- English

使用右上角的"Language"按钮切换语言。

Switch languages using the "Language" button in the top-right corner.

---

## 注意事项
## Notes

- 工具自动检测贴图格式（JPG、PNG、EXR 等）
- The tool automatically detects texture formats (JPG, PNG, EXR, etc.)

- 贴图匹配不区分大小写
- Texture matching is case-insensitive

- 如果 .sbs 文件已存在，将被覆盖
- If a .sbs file already exists, it will be overwritten

- 工具会在所选目录中创建"SBS_Output"文件夹
- The tool creates an "SBS_Output" folder in the selected directory

---

## 致谢
## Credits

专为简化 Substance Designer 工作流程而开发。

Developed for streamlining Substance Designer workflow.

**版本**: 1.0  
**Version**: 1.0

**平台**: Windows  
**Platform**: Windows

**许可**: 免费使用  
**License**: Free to use
