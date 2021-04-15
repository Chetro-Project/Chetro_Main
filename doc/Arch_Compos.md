# [桜斗/Chetro 研究開発要領 基本計画書](./Dev_Base.md)付属書 基本アーキテクチャ(構成システム)構想

## 共通部分

- Kernel: "桜核" a.k.a. "CT-Kernel" or "Ohkaku"
- Daemon: ""
- 1st Boot Loader: "夜明け" a.k.a. "Yoake"
- 2nd Boot Loader: "日の出" a.k.a. "Hinode"
- Continuous Working System: "白夜" a.k.a "Byakuya"

## デスクトップ系列

### - 基礎システム

- Package Manager: "Harding-Io" from "FunCobal family project"
- Software Builder: "Harding-Musubi"(産日) from "FunCobal family project"
- Software Installer: "Harding-Kumihimo"(組紐) from "FunCobal family project"
- Tool Chain: ""
- Terminal: "General Terminal System" a.k.a. "GTS"
- Shell Manager: "Pantheon"
- Standard Shell: "FunCobal Shell " a.k.a. "cosh" from "FunCobal family project"

### - GUI 関係

- Window System : ""
- Desktop Manager: "" as Desktop Environment
- Window Manager: ""
- Rust/Dart GUI Framework/Engine: "Magnarga"
- Graphic System: "鋭像"　 a.k.a. "Eizo" or "Eizo Graphic" ,as 2D/3D Graphic API
- Multi-dimension Driven API: ""

### - 入出力関係

- Text Services Framework: "TR-TSF"
- Japanese & Han-zi-area IME: "Nori IME" from "Nori Project", or "Japanist IME" powered by "Fujitsu"
- General IME: "今昔多国語" a.k.a. "Takokugo"

### - ネットワーク関連

- Network Tracker & Manager: ""
- Internet Communication Terminal System: ""
- Partial Network Domain Manager: ""
- Network Devices Manager Module: ""

### - デバイス関連

- Device Driver Module Loader: "ctd.drive"
- Device Directory Manager: "ctd.dir"
- Inter-Device Transporter Module: "ctd.trans"

#### 内部カード系

- SATA Card Driver Module: "sata.ddm"
- HardDisc IDE Driver Module: "ide.ddm" for IDE, Pin
- Display Graphics Driver Module: "stdGraphica.ddm"
- Graphic RAID Driver Module: "raidGraphica.ddm"

#### I/O 系

- RS Serial Parallel Driver Module: "rsSub.ddm" for RS-232
- Radio Frequency Driver Module: "" for RF, BNC, TBC, SMA, SMB etc
- Sound Access Driver Module: "" for Audio uses such as RCA, DIN, S/PDIF, Phone
- Scanner Access Driver Module: "scanner.ddm" for scanners
- Printer Access Driver Module: "printer.ddm" for printers
- Optical Access Driver Module: "optics.ddm" for S/PDIF, AES/EBU etc
- Multimedia Display Driver Module: "mediaDocker.ddm" for HDMI, DisplayPort, VGA, DVI, BNC, RCA, SCART etc

#### Bus 系

- Card Bus Driver Module: "cardBus.ddm" for PCCard, ExpressCard
- Thunderbolt USB Driver Module: "thunder.ddm" for High-speed USB, Thunderbolt, FireWare
- USB Bus Driver Module: "std_usb.ddm" for default USB
- PCIE Bus Driver Module: "pcie.ddm" for PCIE

### - 標準エンジン

- Application Engine: ""
- Javascript Engine: "boa"
- Dart Engine: ""
- Julia Engine: ""
- Java Engine: ""
- .exe Engine: "窓許" a.k.a. "Madomoto"
- Unix-like OS VM: "Nixer"

### - 基本アプリケーション

- Standard Browser: "Cyclox"
- Extendible Text Editor: ""
- Integlated Painter: ""
- Multi-computer-language Manager: "Onth"
- Office Suite: "書院" a.k.a. "Shoin" powered by "Sharp Co." with "Sun-OpenOffice .org" powered by "Sun Microsystems Co."
  - Writer: "文案" a.k.a. "Bun-an"
  - Spreadsheet: "算表" a.k.a. "San-pyou"
  - Presentation Documents: "演資" a.k.a. "En-shi"
  - Presentation Screens: "演台" a.k.a. "En-dai"
  - Drawer: "図案" a.k.a. "Zu-an"
  - Math Worker: "算板" a.k.a. "San-ban"
  - Forms Worker: "調査票" a.k.a. "Chou-sa-hyou"
  - Teams Collaborator: "組班" a.k.a "Kumi-han"
  - Project Manager: "事業" a.k.a. "Ji-gyou"
  - Planner: "計画" a.k.a. "Kei-kaku"
  - Task Manager: "任務" a.k.a. "Nin-mu"
  - DTP Worker: "書版" a.k.a. "Sho-han"
  - Video Streamer: "映像" a.k.a. "Ei-zo"

## 組込み系列

- Application-Loader:
