<p align="center">
  <img width="180" src="./public/logo.png" alt="ChatGPT">
  <h1 align="center">ChatGPT</h1>
  <p align="center">ChatGPT Masaüstü Uygulaması (Mac, Windows, ve Linux üzerinden erişilebilir)</p>
</p>

[![Turkish badge](https://img.shields.io/badge/%E3%83%88%E3%83%AB%E3%82%B3%E8%AA%9E-Turkish-red)](./README-TR.md)
[![English badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README.md)
[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README-ZH_CN.md)\
[![ChatGPT downloads](https://img.shields.io/github/downloads/lencx/ChatGPT/total.svg?style=flat-square)](https://github.com/lencx/ChatGPT/releases)
[![chat](https://img.shields.io/badge/chat-discord-blue?style=flat&logo=discord)](https://discord.gg/aPhCRf4zZr)
[![twitter](https://img.shields.io/badge/follow-lencx__-blue?style=flat&logo=Twitter)](https://twitter.com/lencx_)
[![youtube](https://img.shields.io/youtube/channel/subscribers/UC__gTZL-OZKDPic7s_6Ntgg?style=social)](https://www.youtube.com/@lencx)

<a href="https://www.buymeacoffee.com/lencx" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 40px !important;width: 145px !important;" ></a>

---
**Bu resmi olmayan proje sadece kişisel öğrenme ve araştırma amaçlı yapılmıştır. ChatGPT'nin masaüstü uygulaması açık kaynaklı olduğundan beri çok fazla ilgi topladı ve bu ilgiden dolayı herkese teşekkür etmek istiyorum. Fakat bu süreçte iki temel sorun gelecekteki gelişmelere büyük ölçüde etki etti:**

- **Bazı sürümler yeniden paketlendi ve kâr amacıyla satıldı.**
- **ChatGPT'nin ismini ve logosunu kullandığım için ihlal anlaşmazlıkları ortaya çıkabilir.**  

**Yeni 'repository' için: https://github.com/lencx/nofwl**

## Canlı Demo

- [ChatGPT Desktop Application v1.0.0](https://youtu.be/IIuuB5vFFAQ)
- [ChatGPT automatically performs the "Continue generating" button, freeing up your hands.](https://youtu.be/bbL5cPmiGig)

## 📦 İndir

- [📝 Update Log](./UPDATE_LOG.md)
- [🕒 History versions...](https://github.com/lencx/ChatGPT/releases)

<!-- tr-download-start -->

### Windows

- [ChatGPT_1.1.0_windows_x86_64.msi](https://github.com/lencx/ChatGPT/releases/download/v1.1.0/ChatGPT_1.1.0_windows_x86_64.msi): Direkt indirme
- [winget](https://winstall.app/apps/lencx.ChatGPT)'i kullanmak için:

  ```bash
  # son sürümü indirme
  winget install --id=lencx.ChatGPT -e

  # belirli bir sürümü indirme
  winget install --id=lencx.ChatGPT -e --version 1.1.0
  ```
**Not : Eğer indirilen yol ve uygulama ismi tamamen aynıysa, bir çakışmayla karşılaşırsınız ([#142](https://github.com/lencx/ChatGPT/issues/142))**

### Mac

- [ChatGPT_1.1.0_macos_aarch64.dmg](https://github.com/lencx/ChatGPT/releases/download/v1.1.0/ChatGPT_1.1.0_macos_aarch64.dmg): Direkt indirme
- [ChatGPT_1.1.0_macos_x86_64.dmg](https://github.com/lencx/ChatGPT/releases/download/v1.1.0/ChatGPT_1.1.0_macos_x86_64.dmg): Direkt indirme
- Homebrew \
 Ya da _[Homebrew](https://brew.sh) ([Cask](https://docs.brew.sh/Cask-Cookbook))_ ile de indirebilirsiniz.:
  ```sh
  brew tap lencx/chatgpt https://github.com/lencx/ChatGPT.git
  brew install --cask chatgpt --no-quarantine
  ```
  Ayrıca eğer _[Brewfile](https://github.com/Homebrew/homebrew-bundle#usage)_ ile şöyle bir şey ekleyebilirsiniz :
  Also, if you keep a _[Brewfile](https://github.com/Homebrew/homebrew-bundle#usage)_, you can add something like this:
  ```rb
  repo = "lencx/chatgpt"
  tap repo, "https://github.com/#{repo}.git"
  cask "chatgpt", args: { "no-quarantine": true }
  ```
**Eğer yazılımı MacOS sistemine indirirken `"ChatGPT" is damaged and can't be opened. You should move it to the Trash` şeklinde bir hatayla karşılaşırsanız sorunun sebebi macOS'taki güvenlik ayarlarından kaynaklanıyor olabilir. Bu sorunu çözebilmek için lütfen şu kodları terminalde çalıştırın:**

```bash
sudo xattr -r -d com.apple.quarantine /YOUR_PATH/ChatGPT.app
```

### Linux

- [ChatGPT_1.1.0_linux_x86_64.deb](https://github.com/lencx/ChatGPT/releases/download/v1.1.0/ChatGPT_1.1.0_linux_x86_64.deb):`.deb` installer olarak indirmek küçük boyuttan dolayı avantajlı ama uyumluluk açısından avantajsız.
- [ChatGPT_1.1.0_linux_x86_64.AppImage.tar.gz](https://github.com/lencx/ChatGPT/releases/download/v1.1.0/ChatGPT_1.1.0_linux_x86_64.AppImage.tar.gz): Güvenilir bir biçimde çalışıyor eğer `.deb` çalışmazsa deneyebilirsiniz.

<!-- tr-download-end -->

## ChatGPT Girdileri!

**[awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)** 'a bakarak uygulamaya eklemek için ilgi çekici yenilikler bulabilirsiniz. Ayrıca 'Sync Prompts'ları da bir tuşla senkronize edebilir ve eğer bazı belirli girdileri slash komutlarında görünmesini istemiyorsanız etkisiz hale getirebilirsiniz.

![chatgpt cmd](./assets/chatgpt-cmd.png)

## ✨ Yenilikler

- `macOS` `Linux` `Windows` için çoklu platform
- Text-to-Speech
- ChatGPT geçmişini "PNG, PDF ve Markdown" olarak dışa aktarma
- Otomatik güncelleme bildirimleri
- Yaygın kısayol tuşları
- System tray hover window
- Güçlü menü eşyaları
- "/" (slash) komutları ve onların konfigürasyonları ( manüel veya dosyayla konfigüre edilebilir [#55](https://github.com/lencx/ChatGPT/issues/55))
- Kişiselleştirilmiş evrensel kısayollar ([#108](https://github.com/lencx/ChatGPT/issues/108))
- Pop-up Aratma ([#122](https://github.com/lencx/ChatGPT/issues/122) "mouse selected" içerik, 400'den fazla karakter desteklemiyor): Uygulama Tauri kullanılarak yapıldı ve güvenlik kısıtlamalarından dolayı bazı şeyler çalışmayabilir o yüzden tarayıcınızı kullanmanızı tavsiye ederiz.

## Teşekkürler

- Genel olarak kullanılan paylaş butonu buradan kopyalandı [@liady](https://github.com/liady) bazı modifikasyonlarla geliştirildi.
[Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts)'a teşekkür ederim. Bu uygulamanın kişiselleştirilmiş komut fonksiyonlarında kaynak olarak ilham alındı
---

[![Star History Chart](https://api.star-history.com/svg?repos=lencx/chatgpt&type=Timeline)](https://star-history.com/#lencx/chatgpt&Timeline)

## 中国用户

国内用户如果遇到使用问题或者想交流 ChatGPT 技巧，可以关注公众号“浮之静”，发送 “chat” 进群参与讨论。公众号会更新[《Tauri 系列》](https://mp.weixin.qq.com/mp/appmsgalbum?__biz=MzIzNjE2NTI3NQ==&action=getalbum&album_id=2593843659863752704)文章，技术思考等等，如果对 tauri 开发应用感兴趣可以关注公众号后回复 “tauri” 进技术开发群（想私聊的也可以关注公众号，来添加微信）。开源不易，如果这个项目对你有帮助可以分享给更多人，或者微信扫码打赏。

<img width="180" src="https://user-images.githubusercontent.com/16164244/207228300-ea5c4688-c916-4c55-a8c3-7f862888f351.png"> <img width="200" src="https://user-images.githubusercontent.com/16164244/207228025-117b5f77-c5d2-48c2-a070-774b7a1596f2.png">

<a href="https://t.zsxq.com/0bQikmcVw"><img width="360" src="./assets/zsxq.png"></a>

## Lisans

AGPL-3.0 License
