# Swarm-UAV-Senkronizasyon-ve-Gorev-Yonetimi

> [!IMPORTANT]
> ## 🔒 Takım Gizliliği ve Kaynak Kod Politikası
>
> Bu proje, takımımıza ve proje ortaklarımıza ait özel bilgi, yöntem ve uygulamaları içermektedir. **Takım gizliliğini, fikrî emeği ve proje güvenliğini korumak amacıyla kaynak kodlar bu depoda paylaşılmamaktadır.**
>
> Bu README; projenin amacı, mimarisi ve kullanılan teknolojiler hakkında genel bir bakış sunar. Kodun tamamı ve ayrıntılı uygulama bileşenleri yalnızca yetkili takım üyelerinin erişimine açıktır.
>
> 📩 Proje hakkında daha fazla bilgi için depo sahibiyle iletişime geçebilirsiniz.

## 📝 Proje Özeti
Birden fazla İnsansız Hava Aracı'nın koordineli ve otonom bir şekilde görev icra etmesini sağlayan merkezi ve dağıtık kontrol sistemidir. Proje, İHA'ların birbirleriyle haberleşerek karmaşık geometrik formasyonlar oluşturmasına ve çarpışmadan görev tamamlamasına odaklanır.

## ✨ Özellikler
* **3B Formasyon Kontrolü:** En az 3 İHA ile V, Çizgi ve Ok Başı (Λ) gibi geometrik düzenlerin korunması.
* **Otonom Navigasyon:** Belirlenen rota üzerinde sürü yapısını bozmadan otonom hareket kabiliyeti.
* **Dinamik Sürü Yönetimi:** Görev esnasında sürüye yeni birey ekleme veya mevcut bireyi çıkarma yeteneği.
* **Çarpışma Önleme:** ORCA algoritmaları ve komşu takibi ile İHA'lar arası güvenli mesafe yönetimi.

## 🛠 Kullanılan Teknolojiler
* **Yazılım:** ROS (Robot Operating System), Gazebo (Simülasyon), Python, C++, MAVLink.
* **Donanım:** Pixhawk 6X, NVIDIA Jetson Xavier NX, CubeOrange.

## 🏗 Proje Yapısı ve Mimarisi
* **Dağıtık Sürü Algoritması:** Merkezi bir kontrol noktası olmadan İHA'ların komşularıyla haberleşerek karar verdiği yapı.
* **Simülasyon Entegrasyonu:** Gerçek uçuş öncesi algoritmaların Gazebo ve MATLAB ortamlarında doğrulanması.
* **Görev Yöneticisi:** Sürü keşif ve formasyon modları arasındaki geçişleri yöneten ana katman.
