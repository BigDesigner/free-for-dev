# free-for.dev

Geliştiriciler ve Açık Kaynak yazarları artık ücretsiz katmanlar sunan birçok hizmete sahip ancak bunların hepsini bulmak, bilinçli kararlar vermek için zaman alıyor.

Bu, yazılımların (SaaS, PaaS, IaaS vb.) ve ücretsiz geliştirici katmanlarına sahip diğer tekliflerin bir listesidir.

Bu özel listenin kapsamı, altyapı geliştiricilerinin (Sistem Yöneticisi, DevOps Uygulayıcıları vb.) yararlı bulacağı şeylerle sınırlıdır. Piyasadaki tüm ücretsiz hizmetleri seviyoruz, ancak konuyu gündemde tutmak iyi olur. Bu bazen gri bir çizgidir, dolayısıyla bu önyargılıdır; Eğer katkınızı kabul etmezsem lütfen gücenmeyin.

Bu liste, 1600'den fazla kişinin katkılarıyla oluşmuştur. Yeni hizmetler eklemek veya bilgileri güncellemek için [depo üzerinden katkıda bulunabilirsiniz](https://github.com/BigDesigner/free-for-dev).

**NOT**: Bu liste yalnızca Hizmet olarak sunulan teklifler içindir, şirket içinde barındırılan yazılımlar için geçerli değildir. Bir hizmetin uygun olabilmesi için yalnızca ücretsiz deneme sürümü değil, ücretsiz katman da sunması gerekir. Zaman aralıklı ise ücretsiz kullanım en az bir yıl sürmelidir. Ücretsiz katmanı güvenlik açısından da değerlendiriyoruz, dolayısıyla SSO uygundur ancak TLS'yi yalnızca ücretli katmanlarla sınırlayan hizmetleri kabul etmeyeceğim.

<a id="table-of-contents"></a>

# İçindekiler

  * [Önemli Bulut Sağlayıcılarının Daima Ücretsiz Sınırları](#major-cloud-providers)
  * [Bulut yönetimi çözümleri](#cloud-management-solutions)
  * [Analitikler, Etkinlikler ve İstatistikler](#analytics-events-and-statistics)
  * [API'ler, Veriler ve ML](#apis-data-and-ml)
  * [Yapı Depoları](#artifact-repos)
  * [BaaS](#baas)
  * [Düşük Kodlu Platform](#low-code-platform)
  * [CDN ve Koruma](#cdn-and-protection)
  * [CI ve CD](#ci-and-cd)
  * [İYS](#cms)
  * [Kod Oluşturma](#code-generation)
  * [Kod Kalitesi](#code-quality)
  * [Kod Arama ve Tarama](#code-search-and-browsing)
  * [Kilitlenme ve İstisna İşleme](#crash-and-exception-handling)
  * [Haritalarda Veri Görselleştirme](#data-visualization-on-maps)
  * [Yönetilen Veri Hizmetleri](#managed-data-services)
  * [Tasarım ve Kullanıcı Arayüzü](#design-and-ui)
  * [Geliştirici Blog Siteleri](#dev-blogging-sites)
  * [DNS](#dns)
  * [Docker'la İlgili](#docker-related)
  * [Etki alanı](#domain)
  * [Eğitim ve Kariyer Gelişimi](#education-and-career-development)
  * [E-posta](#email)
  * [Özellik Yönetim Platformlarını Değiştirir](#feature-toggles-management-platforms)
  * [Yazı tipi](#font)
  * [Formlar](#forms)
  * [Üretken Yapay Zeka](#generative-ai)
  * [IaaS](#iaas)
  * [IDE ve Kod Düzenleme](#ide-and-code-editing)
  * [Uluslararası Cep Telefonu Numarası Doğrulama API'si ve SDK'sı](#international-mobile-number-verification-api-and-sdk)
  * [Sorun Takibi ve Proje Yönetimi](#issue-tracking-and-project-management)
  * [Günlük Yönetimi](#log-management)
  * [Mobil Uygulama Dağıtımı ve Geri Bildirim](#mobile-app-distribution-and-feedback)
  * [Yönetim Sistemleri](#management-system)
  * [Mesajlaşma ve Akış](#messaging-and-streaming)
  * [Çeşitli](#miscellaneous)
  * [İzleme](#monitoring)
  * [PaaS](#paas)
  * [Paket Oluşturma Sistemi](#package-build-system)
  * [Ödeme ve Faturalandırma Entegrasyonu](#payment-and-billing-integration)
  * [Gizlilik Yönetimi](#privacy-management)
  * [Ekran görüntüsü API'leri](#screenshot-apis)
  * [Flutter ile İlgili ve Mac Olmadan IOS Uygulamaları Oluşturma](#flutter-related-and-building-ios-apps-without-mac)
  * [Arama](#search)
  * [Güvenlik ve PKI](#security-and-pki)
  * [Kimlik Doğrulama, Yetkilendirme ve Kullanıcı Yönetimi](#authentication-authorization-and-user-management)
  * [Kaynak Kodu Depoları](#source-code-repos)
  * [Depolama ve Medya İşleme](#storage-and-media-processing)
  * [Tünel Açma, WebRTC, Web Soket Sunucuları ve Diğer Yönlendiriciler](#tunneling-webrtc-web-socket-servers-and-other-routers)
  * [Test ediliyor](#testing)
  * [Ekipler ve İşbirliği için Araçlar](#tools-for-teams-and-collaboration)
  * [Çeviri Yönetimi](#translation-management)
  * [Ziyaretçi Oturumu Kaydı](#visitor-session-recording)
  * [Web Barındırma](#web-hosting)
  * [Yorum Yapma Platformları](#commenting-platforms)
  * [Tarayıcı tabanlı donanım emülasyonu](#browser-based-hardware-emulation-written-in-javascript)
  * [Uzak Masaüstü Araçları](#remote-desktop-tools)
  * [Oyun Geliştirme](#game-development)
  * [Diğer Ücretsiz Kaynaklar](#other-free-resources)

## Major Cloud Providers

  * [Google Bulut Platformu](https://cloud.google.com)
    * App Engine - Günde 28 ön uç örnek saati, günde dokuz arka uç örnek saati
    * Cloud Firestore - 1 GB depolama, günde 50.000 okuma, 20.000 yazma, 20.000 silme
    * Compute Engine - 1 öncelikli olmayan e2-micro, 30 GB HDD, 5 GB anlık görüntü depolama (belirli bölgelerle sınırlıdır), Kuzey Amerika'dan tüm bölge hedeflerine (Çin ve Avustralya hariç) ayda 1 GB ağ çıkışı
    * Bulut Depolama - 5 GB, 1 GB ağ çıkışı
    * Cloud Shell - 5 GB kalıcı depolama alanına sahip web tabanlı Linux kabuğu/birincil IDE. Haftada 60 saat sınırı
    * Cloud Pub/Sub - ayda 10 GB mesaj
    * Bulut İşlevleri - ayda 2 milyon çağrı (hem arka plan hem de HTTP çağrılarını içerir)
    * Cloud Run - Ayda 2 milyon istek, 360.000 GB saniye bellek, 180.000 vCPU saniye işlem süresi, Kuzey Amerika'dan ayda 1 GB ağ çıkışı
    * Google Kubernetes Engine - Bir bölgesel küme için küme yönetimi ücreti yoktur. Her kullanıcı düğümünden standart Compute Engine fiyatlandırması üzerinden ücret alınır
    * BigQuery - Ayda 1 TB sorgulama, her ay 10 GB depolama alanı
    * Cloud Build - günde 120 derleme dakikası
    * Bulut Kaynak Depoları - 5 Kullanıcıya Kadar, 50 GB Depolama, 50 GB Çıkış
    * [Google Colab](https://colab.research.google.com/) - Ücretsiz Jupyter Notebooks geliştirme ortamı.
    * [Firebase Studio](https://firebase.studio) Google Firebase Studio (eski adıyla Project IDX). Google Cloud'da çalışan çevrimiçi VSCode.
    * Tam, ayrıntılı liste - https://cloud.google.com/free

  * [Amazon Web Hizmetleri](https://aws.amazon.com)
    * [CloudFront](https://aws.amazon.com/cloudfront/) - Ayda 1 TB çıkış ve ayda 2 milyon İşlev çağrısı
    * [CloudWatch](https://aws.amazon.com/cloudwatch/) - 10 özel ölçüm ve on alarm
    * [CodeBuild](https://aws.amazon.com/codebuild/) - Aylık 100 dakikalık derleme süresi
    * [CodeCommit](https://aws.amazon.com/codecommit/) - 5 aktif kullanıcı, 50 GB depolama alanı ve ayda 10.000 istek
    * [CodePipeline](https://aws.amazon.com/codepipeline/) - ayda 1 etkin ardışık düzen
    * [DynamoDB](https://aws.amazon.com/dynamodb/) - 25 GB NoSQL Veritabanı
    * [EC2](https://aws.amazon.com/ec2/) - ayda 750 saat t2.micro veya t3.micro(12ay). Ayda 100 GB çıkış
    * [EBS](https://aws.amazon.com/ebs/) - Ayda 30 GB Genel Amaçlı (SSD) veya Manyetik(12 ay)
    * [Elastik Yük Dengeleme](https://aws.amazon.com/elasticloadbalancing/) - ayda 750 saat(12 ay)
    * [RDS](https://aws.amazon.com/rds/) - ayda 750 saat db.t2.micro, db.t3.micro veya db.t4g.micro, 20 GB Genel Amaçlı (SSD) depolama, 20 GB depolama yedeklemesi (12 ay)
    * [S3](https://aws.amazon.com/s3/) - 5 GB Standart nesne depolama, 20 Bin Alma isteği ve 2 Bin Koyma isteği (12 ay)
    * [Buzul](https://aws.amazon.com/glacier/) - 10 GB uzun vadeli nesne depolama
    * [Lambda](https://aws.amazon.com/lambda/) - ayda 1 milyon istek
    * [SNS](https://aws.amazon.com/sns/) - ayda 1 milyon yayınlama
    * [SES](https://aws.amazon.com/ses/) - ayda 3.000 mesaj (12 ay)
    * [SQS](https://aws.amazon.com/sqs/) - 1 milyon mesajlaşma kuyruğu isteği
    * Tam, ayrıntılı liste - https://aws.amazon.com/free/

  * [Microsoft Azure](https://azure.microsoft.com)
    * [Sanal Makineler](https://azure.microsoft.com/services/virtual-machines/) - 1 B1S Linux VM, 1 B1S Windows VM (12 ay)
    * [Uygulama Hizmeti](https://azure.microsoft.com/services/app-service/) - 10 web, mobil veya API uygulaması (60 CPU dakikası/gün)
    * [İşlevler](https://azure.microsoft.com/services/functions/) - ayda 1 milyon istek
    * [DevTest Labs](https://azure.microsoft.com/services/devtest-lab/) - Hızlı, kolay ve yalın geliştirme-test ortamlarını etkinleştirin
    * [Active Directory](https://azure.microsoft.com/services/active-directory/) - 500.000 nesne
    * [Active Directory B2C](https://azure.microsoft.com/services/active-directory/external-identities/b2c/) - 50.000 aylık kayıtlı kullanıcı
    * [Azure DevOps](https://azure.microsoft.com/services/devops/) - 5 aktif kullanıcı, sınırsız özel Git depoları
    * [Azure Pipelines](https://azure.microsoft.com/services/devops/pipelines/) - Linux, macOS ve Windows için açık kaynak için sınırsız dakikaya sahip 10 ücretsiz paralel iş
    * [Microsoft IoT Hub](https://azure.microsoft.com/services/iot-hub/) - günde 8.000 ileti
    * [Yük Dengeleyici](https://azure.microsoft.com/services/load-balancer/) - 1 ücretsiz genel yük dengeli IP (VIP)
    * [Bildirim Merkezleri](https://azure.microsoft.com/services/notification-hubs/) - 1 milyon anlık bildirim
    * [Bant genişliği](https://azure.microsoft.com/pricing/details/bandwidth/) - Ayda 15 GB Gelen (12 ay) ve 5 GB çıkış
    * [Cosmos DB](https://azure.microsoft.com/services/cosmos-db/) - 25 GB depolama ve 1000 RU sağlanan aktarım hızı
    * [Statik Web Uygulamaları](https://azure.microsoft.com/pricing/details/app-service/static/) - Ücretsiz SSL, Kimlik Doğrulama/Yetkilendirme ve özel alan adlarıyla statik uygulamalar ve sunucusuz işlevler oluşturun, dağıtın ve barındırın
    * [Depolama](https://azure.microsoft.com/services/storage/) - 5 GB LRS Dosyası veya Blob depolama (12 ay)
    * [Bilişsel Hizmetler](https://azure.microsoft.com/services/cognitive-services/) - Sınırlı işlemler dahil ücretsiz kullanıma sahip AI/ML API'leri (Bilgisayarlı Görüntü, Çevirmen, Yüz algılama, Botlar vb.)
    * [Bilişsel Arama](https://azure.microsoft.com/services/search/#features) - Yapay zeka tabanlı arama ve indeksleme hizmeti, 10.000 belge için ücretsiz
    * [Azure Kubernetes Service](https://azure.microsoft.com/services/kubernetes-service/) - Yönetilen Kubernetes hizmeti, ücretsiz küme yönetimi
    * [Event Grid](https://azure.microsoft.com/services/event-grid/) - 100.000 işlem/ay
    * Tam, ayrıntılı liste - https://azure.microsoft.com/free/

  * [Oracle Bulutu](https://www.oracle.com/cloud/)
    * Hesapla
       - Her biri 1/8 OCPU ve 1 GB belleğe sahip 2 AMD tabanlı Bilgi İşlem VM'si
       - 4 Arm tabanlı Ampere A1 çekirdeği ve tek bir VM veya 4'e kadar VM olarak kullanılabilen 24 GB bellek
       - Örnekler [boşta sayıldığında](https://docs.oracle.com/en-us/iaas/Content/FreeTier/freetier_topic-Always_Free_Resources.htm#compute__idleinstances) geri alınacaktır.
    * Blok Hacmi - 2 cilt, toplam 200 GB (bilgi işlem için kullanılır)
    * Nesne Depolama - 10 GB
    * Yük dengeleyici - 10 Mb/sn ile 1 örnek
    * Veritabanları - 2 DB, her biri 20 GB
    * İzleme - 500 milyon alım veri noktası, 1 milyar alma veri noktası
    * Bant genişliği - Ayda 10 TB çıkış, x64 tabanlı VM'de hız 50 Mbps ile sınırlıdır, ARM tabanlı VM'de 500 Mbps* çekirdek sayısı
    * Genel IP - VM'ler için 2 IPv4, yük dengeleyici için 1 IPv4
    * Bildirimler - Ayda 1 milyon teslimat seçeneği, ayda 1000 e-posta gönderilir
    * Tam, ayrıntılı liste - https://www.oracle.com/cloud/free/

  * [IBM Bulut](https://www.ibm.com/cloud/free/)
    * Cloudant veritabanı - 1 GB veri depolama alanı
    * Db2 veritabanı - 100 MB veri depolama alanı
    * API Connect - ayda 50.000 API çağrısı
    * Kullanılabilirlik İzleme - ayda 3 milyon veri noktası
    * Günlük Analizi - 500MB günlük günlük
    * Tam, ayrıntılı liste - https://www.ibm.com/cloud/free/

  * [Bulut parlaması](https://www.cloudflare.com/)
    * [Uygulama Hizmetleri](https://www.cloudflare.com/plans/) - Sınırsız sayıda alan adı için ücretsiz DNS, DDoS Koruması, ücretsiz SSL ile birlikte CDN, Güvenlik Duvarı kuralları ve sayfa kuralları, WAF, Bot Azaltma, Ücretsiz Ölçülmemiş Hız Sınırlaması - Alan adı başına 1 kural, Analytics, E-posta yönlendirme
    * [Sıfır Güven ve SASE](https://www.cloudflare.com/plans/zero-trust-services/) - 50 Kullanıcıya kadar, 24 saatlik etkinlik kaydı, üç ağ konumu
    * [Cloudflare Tüneli](https://www.cloudflare.com/products/tunnel/) - Yerel olarak çalışan HTTP bağlantı noktasını bir tünel üzerinden trycloudflare.com'daki rastgele bir alt alana yönlendirebilirsiniz, [Hızlı Tüneller](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/do-more-with-tunnels/trycloudflare/) kullanın, Hesap gerekmez. [Sıfır Güven](https://www.cloudflare.com/products/zero-trust/) Ücretsiz Planında daha fazla özellik (TCP tüneli, Yük dengeleme, VPN).
    * [Workers](https://developers.cloudflare.com/workers/) - Cloudflare'in küresel ağında günlük 100 bin istekte sunucusuz kodu ücretsiz olarak dağıtın.
    * [İşçiler KV](https://developers.cloudflare.com/kv) - Günde 100 bin okuma isteği, günde 1000 yazma isteği, günde 1000 silme isteği, günde 1000 liste isteği, 1 GB depolanan veri
    * [R2](https://developers.cloudflare.com/r2/) - Ayda 10 GB, ayda 1 milyon A Sınıfı işlem, ayda 10 milyon B Sınıfı işlem
    * [D1](https://developers.cloudflare.com/d1/) - Günde 5 milyon satır okunur, günde 100 bin satır yazılır, 1 GB depolama alanı
    * [Pages](https://developers.cloudflare.com/pages/) - Web uygulamalarınızı Cloudflare'in hızlı, güvenli küresel ağında geliştirin ve dağıtın. Beş yüz aylık derleme, 100 özel alan adı, Entegre SSL, sınırsız erişilebilir lisans, sınırsız önizleme dağıtımı ve Cloudflare Workers entegrasyonu aracılığıyla tam yığın yeteneği.
    * [Kuyruklar](https://developers.cloudflare.com/queues/) - ayda 1 milyon işlem
    * [TURN](https://developers.cloudflare.com/calls/turn/) - Ayda 1 TB ücretsiz (giden) trafik.

  * [Zoho](https://www.zoho.com) - Bir e-posta sağlayıcısı olarak başladı ancak artık bazılarının ücretsiz planları olan bir dizi hizmet sunuyor. Ücretsiz planları olan hizmetlerin listesi:
    * [Catalyst by Zoho](https://catalyst.zoho.com) - Cömert bir [ücretsiz katmana](https://catalyst.zoho.com/free-tier.html) sahip PaaS/tam yığın bulut platformu
    * [E-posta](https://zoho.com/mail) 5 kullanıcı için ücretsiz. 5 GB/kullanıcı ve 25 MB ek sınırı, tek alan adı.
    * [Zoho Assist](https://www.zoho.com/assist) - Zoho Assist'in sonsuza kadar ücretsiz planı, bir eşzamanlı uzaktan destek lisansını ve hem profesyonel hem de personel kullanımına yönelik sınırsız süre boyunca 5 gözetimsiz bilgisayar lisansına Erişim içerir.
    * [Sprintler](https://zoho.com/sprints) 5 kullanıcı için ücretsiz, 5 Proje ve 500 MB depolama alanı.
    * [Dokümanlar](https://zoho.com/docs) - 1 GB yükleme sınırı ve 5 GB depolama alanıyla 5 kullanıcı için ücretsiz. Zoho Office Suite (Yazar, E-Tablolar ve Gösteri) paket halinde gelir.
    * [Projeler](https://zoho.com/projects) - 3 kullanıcı için ücretsiz, 2 proje ve 10 MB ek sınırı. Aynı plan [Bugtracker](https://zoho.com/bugtracker) için de geçerlidir.
    * [Bağlan](https://zoho.com/connect) - Üç grup, üç özel uygulama, 3 Pano, 3 Kılavuz ve 10 Entegrasyonun yanı sıra kanallar, etkinlikler ve forumlarla 25 kullanıcı için ücretsiz Ekip İşbirliği.
    * [Toplantı](https://zoho.com/meeting) - En fazla 3 toplantı katılımcısı ve 10 Web Semineri katılımcısıyla toplantılar.
    * [Vault](https://zoho.com/vault) - Şifre Yönetimine Bireyler erişebilir.
    * [Showtime](https://zoho.com/showtime) - 5 katılımcıya kadar uzaktan oturum eğitimi için başka bir Toplantı yazılımı.
    * [Notebook](https://zoho.com/notebook) - Evernote'a ücretsiz bir alternatif.
    * [Wiki](https://zoho.com/wiki) - 50 MB depolama alanı, sınırsız sayfalar, zip yedeklemeleri, RSS ve Atom beslemesi, erişim kontrolleri ve özelleştirilebilir CSS ile üç kullanıcı için ücretsiz.
    * [Abonelikler](https://zoho.com/subscriptions) - Yinelenen Faturalandırma yönetimi, 20 müşteri/abonelik ve 1 kullanıcı için ücretsiz olup, tüm ödeme barındırma hizmetleri Zoho tarafından yapılır. Son 40 abonelik metriği saklanır
    * [Ödeme](https://zoho.com/checkout) - 3 sayfa ve 50'ye kadar ödeme içeren Ürün Faturalandırma yönetimi.
    * [Masa](https://zoho.com/desk) - Üç temsilci, özel bilgi tabanı ve e-posta destek bildirimleriyle Müşteri Desteği yönetimi. Bir uzak teknisyen ve 5 gözetimsiz bilgisayar için [Assist](https://zoho.com/assist) ile entegre olur.
    * [Cliq](https://zoho.com/cliq) - 100 GB depolama alanına, sınırsız kullanıcıya, kanal başına 100 kullanıcıya ve SSO'ya sahip ekip sohbet yazılımı.
    * [Kampanyalar](https://zoho.com/campaigns) - E-postayla Pazarlama
    * [Formlar](https://zoho.com/forms) - Form Oluşturucu
    * [Sign](https://zoho.com/sign) - Kağıtsız İmzalar
    * [Anketler](https://zoho.com/surveys) - Çevrimiçi Anketler
     * [Rezervasyonlar](https://zoho.com/bookings) - Randevu Planlama

**[⬆️Başa Dön](#table-of-contents)**

## Cloud management solutions

  * [Brainboard](https://www.brainboard.co) - Bulut altyapılarını uçtan uca görsel olarak oluşturmak ve yönetmek için ortak çözüm.
  * [Cloud 66](https://www.cloud66.com/) - Kişisel projeler için ücretsiz (bir dağıtım sunucusu, bir statik site içerir), Cloud 66 size "sunucu sorunları" baş ağrısı olmadan herhangi bir bulut üzerinde uygulamalarınızı oluşturmak, dağıtmak ve büyütmek için ihtiyacınız olan her şeyi sağlar.
  * [deployment.io](https://deployment.io) - Deployment.io, geliştiricilerin AWS'deki dağıtımları otomatikleştirmesine yardımcı olur. Ücretsiz katmanımızda bir geliştirici (tek kullanıcı) sınırsız statik site, web hizmeti ve ortam dağıtabilir. Ücretsiz katmana dahil önizlemeler ve otomatik dağıtımlarla ayda 10 iş yürütmeyi ücretsiz sağlıyoruz.
  * [Pulumi](https://www.pulumi.com/) - Bulut altyapısını oluşturmak, dağıtmak ve yönetmek için tanıdık programlama dillerini ve araçlarını kullanmanıza olanak tanıyan bir kod platformu olarak modern altyapı.
  * [scalr.com](https://scalr.com/) - Scalr, Terraform tarafından yönetilen altyapı ve yapılandırmalarda daha iyi işbirliği ve otomasyon sağlamak için kullanılan bir Terraform Otomasyon ve İşbirliği (TACO) ürünüdür. Tam Terraform CLI desteği, OPA entegrasyonu ve hiyerarşik yapılandırma modeli. TOA vergisi yok. Tüm özellikler dahildir. Ayda 50'ye kadar çalıştırmayı ücretsiz kullanın.

**[⬆️Başa Dön](#table-of-contents)**

## Source Code Repos

  * [Bitbucket](https://bitbucket.org/) - Pipelines for CI/CD ile en fazla 5 kullanıcı için sınırsız genel ve özel Git depoları
  * [Codeberg](https://codeberg.org/) - Ücretsiz ve açık kaynaklı projeler için sınırsız genel ve özel Git depoları (sınırsız ortak çalışanla). [Forgejo](https://forgejo.org/) tarafından desteklenmektedir. [Codeberg Pages](https://codeberg.page/) ile statik web sitesi barındırma. [Codeberg'in CI'sı](https://docs.codeberg.org/ci/) ile CI/CD barındırma. Hosting'i [Codeberg Translate](https://translate.codeberg.org/) ile çeviriyorum. Paket ve Konteyner barındırma, Proje yönetimi ve Sorun Takibini içerir
  * [framagit.org](https://framagit.org/) - Framagit, Framasoft'un Gitlab yazılımını temel alan, CI, Statik Sayfalar, Proje sayfaları ve Sorun takibini içeren, geliştirilmiş bir yazılımdır.
  * [GitGud](https://gitgud.io) - Sınırsız özel ve genel depolar. Sonsuza kadar özgür. GitLab ve Sapphire tarafından desteklenmektedir. CI/CD, Statik Barındırma, Konteyner Kaydı, Proje Yönetimi ve Sorun Takibini içerir.
  * [GitHub](https://github.com/) - Sınırsız genel depo ve sınırsız özel depo (sınırsız ortak çalışanla). CI/CD, Geliştirme Ortamı, Statik Barındırma, Paket ve Konteyner barındırma, Proje yönetimi ve AI Copilot'u içerir
  * [gitlab.com](https://about.gitlab.com/) - En fazla 5 ortak çalışanla sınırsız genel ve özel Git depoları. CI/CD, Statik Barındırma, Konteyner Kaydı, Proje Yönetimi ve Sorun Takibini içerir
  * [heptapod.net](https://foss.heptapod.net/) - Heptapod, GitLab Community Edition'ın Mercurial desteği sağlayan dost canlısı bir çatalıdır
  * [Pagure.io](https://pagure.io) - Pagure.io, FOSS lisanslı projeler için Git tabanlı, ücretsiz ve açık kaynaklı bir yazılım kodu işbirliği platformudur
  * [pijul.com](https://pijul.com/) - Sınırsız ücretsiz ve açık kaynaklı dağıtılmış sürüm kontrol sistemi. Ayırt edici özelliği, öğrenilmesini, kullanılmasını ve dağıtılmasını kolaylaştıran sağlam bir yama teorisine dayanmaktadır. Git/hg/svn/darcs'ın birçok sorununu çözer.
  * [projectlocker.com](https://projectlocker.com) - 50 MB alana sahip bir adet ücretsiz özel proje (Git ve Subversion)
  * [RocketGit](https://rocketgit.com) - Git'e dayalı Depo Barındırma. Sınırsız Kamu ve özel depolar.
  * [savannah.gnu.org](https://savannah.gnu.org/) - Özgür Yazılım projeleri için işbirlikçi bir yazılım geliştirme yönetim sistemi olarak hizmet verir (GNU Projeleri için)
  * [savannah.nongnu.org](https://savannah.nongnu.org/) - Özgür Yazılım projeleri için (GNU olmayan projeler için) işbirliğine dayalı bir yazılım geliştirme yönetim sistemi olarak hizmet verir

**[⬆️Başa Dön](#table-of-contents)**

## APIs, Data, and ML

  * [Soyut API](https://www.abstractapi.com) - IP coğrafi konumu, cinsiyet tespiti veya e-posta doğrulama dahil olmak üzere çeşitli kullanım örneklerine yönelik API paketi.
  * [Apify](https://www.apify.com/) - Herhangi bir web sitesi için API oluşturmak ve veri çıkarmak için web kazıma ve otomasyon platformu. Hazır kazıyıcılar, entegre proxy'ler ve özel çözümler. Her ay 5 ABD Doları platform kredisi içeren ücretsiz plan.
  * [APITemplate.io](https://apitemplate.io) - Basit bir API veya Zapier ve Airtable gibi otomasyon araçlarıyla görüntüleri ve PDF belgelerini otomatik olarak oluşturun. CSS/HTML gerekmez. Ücretsiz planda ayda 50 görsel ve üç şablon bulunur.
  * [APIVerve](https://apiverve.com) - Kalite, tutarlılık ve güvenilirlik göz önünde bulundurularak oluşturulmuş 120'den fazla API'ye ücretsiz olarak anında erişim elde edin. Ücretsiz plan ayda 50'ye kadar API Tokenını kapsar. (Muhtemelen kaldırıldı, 2025-06-25)
  * [Arize AI](https://arize.com/) - Model izleme ve veri kalitesi ve performans sapması gibi temel sorunlara neden olan sorunlar için makine öğreniminin gözlemlenebilirliği. İki modele kadar ücretsiz.
  * [Beeceptor](https://beeceptor.com) - Çoklu protokol API'lerini (REST, SOAP, gRPC ve GraphQL) taklit etmek ve hata ayıklamak için kodsuz, bulut tabanlı platform; daha hızlı entegrasyon ve test için kurallara dayalı mantık, CRUD ve durum bilgisi içeren alay etme, proxy oluşturma ve CORS yönetimi ile anlık sunucular sağlar. Ücretsiz plan günde 50 istek içerir ve kontrol paneli URL'sine sahip herkesin gönderilen istekleri ve yanıtları görüntüleyebileceği genel bir kontrol paneli/uç nokta sağlar.
  * [BigDataCloud](https://www.bigdatacloud.com/) - IP Coğrafi Konum Belirleme, Tersine Coğrafi Kodlama, Ağ İçgörüleri, E-posta ve Telefon Doğrulaması, Müşteri Bilgileri ve daha fazlası gibi modern web için hızlı, doğru ve ücretsiz (Sınırsız veya 10.000-50.000'e kadar/ay) API'ler sağlar.
  * [Yapay zekaya göz at](https://www.browse.ai) - Web'deki verileri çıkarma ve izleme. Ayda 1 bin ücretsiz kredi, 1 bin eşzamanlı isteğe eşittir.
  * [BrowserCat](https://www.browsercat.com) - Otomasyon, kazıma, AI aracısı web erişimi, resim/pdf oluşturma ve daha fazlası için başsız tarayıcı API'si. Ayda 1 bin istek içeren ücretsiz plan.
  * [Calendarific](https://calendarific.com) - 200'den fazla ülke için kurumsal düzeyde Resmi tatil API hizmeti. Ücretsiz plan ayda 500 çağrı içerir.
  * [Canopy](https://www.canopyapi.co/) - Amazon.com ürün, arama ve kategori verileri için GraphQL API'si. Ücretsiz plan ayda 100 çağrı içerir.
  * [CarAPI.dev](https://carapi.dev) - VIN kod çözme, çalıntı araç kontrolleri, araç değerleme, muayene verileri ve daha fazlasını içeren kapsamlı otomotiv veri API'si. Ücretsiz katman, 9 uç noktanın tamamında ayda 100 istek içerir.
  * [Cloudmersive](https://cloudmersive.com/) - Ayda 600 çağrı, yalnızca Kuzey Amerika AZ, maksimum 2,5 MB dosya boyutuyla Belge Dönüştürme, Virüs Tarama ve daha fazlasını içeren kapsamlı API Kitaplığına tam erişime sahip Yardımcı Program API platformu.
  * [İşbirliği](https://colab.research.google.com) - Nvidia Tesla K80 GPU'ya sahip ücretsiz web tabanlı Python dizüstü bilgisayar ortamı.
  * [CometML](https://www.comet.com/site/) - Eğitimden üretime kadar iş akışınızı kapsayan, deneme izleme, model üretim yönetimi, model kaydı ve eksiksiz veri kökeni için MLOps platformu. Bireyler ve akademisyenler için ücretsizdir.
  * [Ticaret Katmanı](https://commercelayer.io) - Herhangi bir ön uçtan sipariş oluşturabilen, yerleştirebilen ve yönetebilen şekillendirilebilir ticaret API'si. Geliştirici planı ayda 100 siparişe ve 1.000 SKU'ya kadar ücretsiz olarak izin veriyor.
  * [Composio](https://composio.dev/) - AI Aracıları ve LLM'ler için entegrasyon platformu. Aracı internet üzerinden 200'den fazla aracı entegre edin.
  * [Dönüştürme Araçları](https://conversiontools.io/) - Belgeler, resimler, videolar, sesler ve e-Kitaplar için Çevrimiçi Dosya Dönüştürücü. REST API'si mevcut. Node.js, PHP, Python için kütüphaneler. 50 GB'a kadar dosyaları destekleyin (ücretli planlar için). Ücretsiz katman, dosya boyutuna (20 MB) ve dönüşüm sayısına (30/Gün, 300/Ay) göre sınırlıdır.
  * [Ülke-Eyalet-Şehir Mikro Hizmet API'si](https://country-state-city.rebuscando.info/) - Ülkeler, bölgeler, iller, şehirler, posta kodları ve çok daha fazlasını içeren geniş bir bilgi yelpazesi sağlayan API ve Mikro hizmet. Ücretsiz katman günde en fazla 100 isteği içerir.
  * [Coupler](https://www.coupler.io/) - Uygulamalar arasında senkronizasyon sağlayan veri entegrasyon aracı. Canlı gösterge tabloları ve raporlar oluşturabilir, değerleri dönüştürebilir ve değiştirebilir, içgörüleri toplayıp yedekleyebilir. Ücretsiz plan bir kullanıcı, veri bağlantısı, veri kaynağı ve veri hedefi ile sınırlıdır. Ayrıca manuel veri yenileme gerektirir.
  * [CraftMyPDF](https://craftmypdf.com) - Bırak ve bırak düzenleyicisi ve basit bir API ile yeniden kullanılabilir şablonlardan PDF belgelerini otomatik olarak oluşturun. Ücretsiz plan ayda 100 PDF ve üç şablonla birlikte gelir.
  * [Cube](https://cube.dev/) - Cube, veri mühendislerinin ve uygulama geliştiricilerinin modern veri depolarındaki verilere erişmesine, bunları tutarlı tanımlar halinde düzenlemesine ve her uygulamaya sunmasına yardımcı olur. Cube'u kullanmanın en hızlı yolu, günde 1.000 sorguyla sınırlı ücretsiz katmana sahip olan Cube Cloud'dur.
  * [CurlHub](https://curlhub.io) - API çağrılarını incelemek ve hata ayıklamak için proxy hizmeti. Ücretsiz plan ayda 10.000 istek içerir.
  * [CurrencyScoop](https://currencyscoop.com) - Fintech uygulamaları için gerçek zamanlı para birimi verileri API'si. Ücretsiz plan ayda 5.000 çağrı içerir.
  * [CustomJS](https://www.customjs.io) - HTML'den PDF'ye veya PDF'den PNG/Metin ve PDF'ye birleştirme/çıkarma/birleştirme API'leri. Ücretsiz katmanda ayda 600 çağrı vardır.
  * [Veri Alıcısı](https://datafetcher.com) - Airtable'ı herhangi bir uygulamaya veya API'ye kod olmadan bağlayın. Airtable'da API isteklerini çalıştırmak için postacı benzeri arayüz. Düzinelerce uygulamayla önceden oluşturulmuş entegrasyonlar. Ücretsiz plan ayda 100 çalıştırma içerir.
  * [Veri Madenci](https://dataminer.io/) - CSV veya Excel web sayfalarından veri çıkarmak için bir tarayıcı uzantısı (Google Chrome, MS Edge). Ücretsiz plan size ayda 500 sayfa verir.
  * [Dataimporter.io](https://www.dataimporter.io) - Salesforce'a bağlanmak, temizlemek ve verileri içe aktarmak için kullanılan araç. Ücretsiz Plan ayda 20.000'e kadar kayıt içerir.
  * [Datalore](https://datalore.jetbrains.com) - Jetbrains'in Python not defterleri. Her ay 10 GB depolama alanı ve 120 saatlik çalışma süresi içerir.
  * [DB Designer](https://www.dbdesigner.net/) - 2 Veritabanı modeli ve model başına on tablodan oluşan ücretsiz bir başlangıç ​​planına sahip Bulut tabanlı Veritabanı şeması tasarımı ve modelleme aracı.
  * [DB-IP](https://db-ip.com/api/free) - IP başına günlük 1k istek içeren ücretsiz IP coğrafi konum API'si. CC-BY 4.0 Lisansı kapsamında lite veritabanı da ücretsizdir.
  * [DeepAR](https://developer.deepar.ai) - Tek bir SDK'ya sahip herhangi bir platform için artırılmış gerçeklik yüz filtreleri. Ücretsiz plan, aylık 10'a kadar aktif kullanıcı (MAU) sağlar ve 4 yüze kadar izleme sağlar
  * [Deepnote](https://deepnote.com) - Yeni bir veri bilimi not defteri. Jupyter, gerçek zamanlı işbirliği ve bulutta çalışmayla uyumludur. Ücretsiz katman, sınırsız kişisel projeleri, 5 GB RAM ve 2vCPU'lu sınırsız temel makineleri ve en fazla 3 düzenleyiciye sahip ekipleri içerir.
  * [JSON'u Karşılaştır](https://comparejson.com) - İki JSON veri yapısı arasındaki farkları karşılaştıran ve JSON verilerindeki farkları hızlı bir şekilde bulmanıza yardımcı olan çevrimiçi bir araç.
  * [Disease.sh](https://disease.sh/) - Covid-19 ile ilgili faydalı Uygulamalar oluşturmak için doğru veriler sağlayan ücretsiz bir API.
  * [Doczilla](https://www.doczilla.app/) - Doğrudan HTML/CSS/JS kodundan ekran görüntüleri veya PDF'ler oluşturulmasını sağlayan SaaS API'si. Ücretsiz plan ayda 250 belgeye izin verir.
  * [Doppio](https://doppio.sh/) - En iyi işleme teknolojisini kullanarak PDF'ler ve Ekran Görüntüleri oluşturmak ve özel olarak depolamak için yönetilen API. Ücretsiz plan ayda 400 PDF ve Ekran Görüntüsüne izin verir.
  * [drawDB](https://drawdb.app/) - Kayıt gerektirmeyen ücretsiz ve açık kaynaklı çevrimiçi veritabanı şeması düzenleyicisi.
  * [DynamicDocs](https://advicement.io) - LaTeX şablonlarını temel alan JSON'dan PDF'ye API ile PDF belgeleri oluşturun. Ücretsiz plan, ayda 50 API çağrısına ve bir şablon kitaplığına erişime izin verir.
  * [Kazanç Akışı](https://earningsfeed.com/api) - Gerçek zamanlı SEC kayıtları, içeriden bilgi ticareti ve kurumsal holdingler API'si. Ücretsiz katman, dakikada 15 istek içerir.
  * [SDK'yı Dışa Aktar](https://exportsdk.com) - Bir SDK ve kod içermeyen entegrasyonlar sağlayan, sürükle ve bırak şablon düzenleyicisine sahip PDF oluşturucu API'si. Ücretsiz planda 250 aylık sayfa, sınırsız kullanıcı ve üç şablon bulunur.
  * [ExtendsClass](https://extendsclass.com/rest-client-online.html) - HTTP isteklerini göndermek için ücretsiz web tabanlı HTTP istemcisi.
  * [Finansal Veriler](https://financialdata.net/) - Borsa ve finansal veriler API'si. Ücretsiz plan günde 300 isteğe izin verir.
  * [FormatJSONOnline.com](https://formatjsononline.com) - JSON verilerini anında biçimlendirmek, doğrulamak, karşılaştırmak ve küçültmek için ücretsiz, tarayıcı tabanlı bir araç.
  * [FraudLabs Pro](https://www.fraudlabspro.com) - Kredi kartı ödeme sahtekarlığı için bir sipariş işlemini tarayın. Bu REST API, bir siparişin giriş parametrelerine göre olası tüm dolandırıcılık özelliklerini tespit edecektir. Ücretsiz Mikro planında ayda 500 işlem bulunur.
  * [FreeIPAPI](https://freeipapi.com) - JSON'da ticari ve ticari olmayan kullanıcılar için Ücretsiz, Hızlı ve Güvenilir IP Coğrafi Konum API'si mevcuttur
  * [Geolocate.io](https://geolocated.io) - Çok kıtalı sunuculara sahip IP Geolocation API'si, günde 2.000 istekle ücretsiz bir plan sunar.
  * [Hex](https://hex.tech/) - not defterleri, veri uygulamaları ve bilgi kitaplıkları için ortak çalışmaya dayalı bir veri platformu. Beş projeye kadar ücretsiz topluluk katmanı.
  * [Hook0](https://www.hook0.com/) - Hook0, çevrimiçi ürünlerin web kancaları sağlamasını kolaylaştıran açık kaynaklı bir hizmet olarak Web kancasıdır (WaaS). Yedi günlük geçmiş saklama özelliğiyle günde 100'e kadar olayı ücretsiz olarak gönderin.
  * [Hoppscotch](https://hoppscotch.io) - Ücretsiz, hızlı ve güzel bir API istek oluşturucu.
  * [HS Ping](https://hsping.com) - Günde 100 arama sunan ücretsiz bir planla, çok ülkeli bir HS (Harmonize Sistem) ve HTS (Harmonize Tarife Sistemi) kod arama API'si.
  * [huggingface.co](https://huggingface.co) - Pytorch, TensorFlow ve JAX için NLP modelleri oluşturun, eğitin ve dağıtın. Ayda 30.000'e kadar giriş karakteri ücretsiz.
  * [Insomnia](https://insomnia.rest) - API'leri tasarlamak ve test etmek için açık kaynaklı API istemcisi; REST ve GraphQL'i destekler
  * [Invantive Cloud](https://cloud.invantive.com/) - Invantive SQL veya OData4 (genellikle Power BI veya Power Query) kullanarak Exact Online, Twinfield, ActiveCampaign veya Visma gibi 70'in üzerinde (bulut) platforma erişin. Veri çoğaltma ve değişimini içerir. Geliştiriciler ve uygulama danışmanları için ücretsiz plan. Veri hacimlerinde sınırlamalar bulunan belirli platformlar için ücretsizdir.
  * [ipwho.org'dan IP Coğrafi Konum API'si](https://ipwho.org/) - Günde 2.000 ücretsiz istek. Kurumsal olmayan fiyatlarla hızlı, kurumsal düzeyde API. Geliştiriciler, şirketler, hükümet ve eğitim müşterileri tarafından güvenilmektedir. 12'den fazla bölgedeki sunucular.
  * [IP Geolocation API](https://www.abstractapi.com/ip-geolocation-api) - Abstract'tan IP Geolocation API'si - 1.000 ücretsiz isteğe izin verir.
  * [IP Geolocation](https://ipgeolocation.io/) - IP Geolocation API - Geliştiriciler için günlük 1.000 istek sınırıyla sonsuza kadar ücretsiz plan.
  * [ip-api](https://ip-api.com) - IP Coğrafi Konum API'si, Ticari olmayan kullanım için ücretsiz, API anahtarı gerekmez, ücretsiz plan için aynı IP adresinden 45 istek/dakika ile sınırlıdır.
  * [IP.City](https://ip.city) - Günde 100 Ücretsiz IP coğrafi konum isteği
  * [IP2Location.io](https://www.ip2location.io/) - Ücretsiz, hızlı ve güvenilir IP coğrafi konum API'si. Şehir, koordinatlar, ISP, ASN, AS verileri ve daha fazlası gibi verileri alın. Ücretsiz plan ayda 50 bin kredi içerir. IP2Location.io ayrıca ayda 500 ücretsiz WHOIS ve barındırılan alan adı araması sunar. Alan kaydı ayrıntılarına bakın ve belirli bir IP'de barındırılan alan adlarını bulun. Daha fazla özellik için ücretli plana geçin.
  * [ipaddress.sh](https://ipaddress.sh) - Farklı [biçimlerde](https://about.ipaddress.sh/) genel bir IP adresi almaya yönelik basit hizmet.
  * [ipapi.is](https://ipapi.is/) - Geliştiriciler için Geliştiriciler tarafından sunulan, mevcut en iyi Barındırma Algılama özelliklerine sahip güvenilir bir IP Adresi API'si. Ücretsiz plan, kayıt olmadan 1000 arama sunar.
  * [ipapi](https://ipapi.co/) - Kloudend, Inc. tarafından sunulan IP Adresi Konum API'si - Fortune 500 tarafından güvenilen, AWS üzerinde oluşturulmuş güvenilir bir coğrafi konum API'sidir. Ücretsiz katman, kaydolmadan ayda 30 bin arama (1 bin/gün) sunar.
  * [ipbase.com](https://ipbase.com) - IP Coğrafi Konum API'si - 150 aylık isteği kapsayan, sonsuza kadar ücretsiz plan.
  * [IPinfo](https://ipinfo.io/) - Hızlı, doğru ve ücretsiz (ayda 50.000'e kadar) IP adresi veri API'si. Coğrafi konum, şirketler, operatörler, IP aralıkları, alanlar, kötüye kullanım kişileri ve daha fazlası hakkında ayrıntılı bilgi içeren API'ler sunar. Tüm ücretli API'ler ücretsiz olarak denenebilir.
  * [IPLocate](https://www.iplocate.io) - IP Coğrafi Konum API'si, günde 1.000 isteğe kadar ücretsiz. Proxy/VPN/barındırma algılamayı, ASN verilerini, Şirket IP'sini ve daha fazlasını içerir. IPLocate ayrıca CSV veya GeoIP uyumlu MMDB formatlarında Ülkeye ve IP'den ASN veritabanlarına ücretsiz indirilebilir IP sunar.
  * [IPTrace](https://iptrace.io) - Ayda 50.000 ücretsiz aramayla işletmenize güvenilir ve yararlı IP coğrafi konum verileri sağlayan utanç verici derecede basit bir API.
  * [JSON IP](https://getjsonip.com) - Talep edilen istemcinin Genel IP adresini döndürür. Ücretsiz seviye için kayıt gerekmemektedir. CORS kullanılarak veriler, istemci tarafı JS kullanılarak doğrudan tarayıcıdan talep edilebilir. İstemci ve sunucu IP'lerindeki değişiklikleri izleyen hizmetler için kullanışlıdır. Sınırsız İstekler.
  * [JSON'dan Tabloya](https://jsontotable.org) - Çevrimiçi hızlı görüntüleme, düzenleme ve paylaşım için JSON'u etkileşimli bir tabloya dönüştürün.
  * [JSON2Video](https://json2video.com) - Video pazarlamayı ve sosyal medya videolarını programlı olarak veya kodsuz olarak otomatikleştirmek için bir video düzenleme API'si.
  * [JSONGrid](https://jsongrid.com) - Karmaşık JSON verilerini güzel tablolu Izgarada Görselleştirmek, Düzenlemek ve Filtrelemek için ücretsiz araç. JSON verilerini bağlantı bağlantısı üzerinden kaydedin ve paylaşın.
  * [JSONing](https://jsoning.com/api/) - Bir JSON nesnesinden sahte bir REST API oluşturun ve HTTP durum kodlarını, başlıkları ve yanıt gövdelerini özelleştirin.
  * [JSONSwiss](https://www.jsonswiss.com/) - JSONSwiss, güçlü bir çevrimiçi JSON görüntüleyici, düzenleyici ve doğrulayıcıdır. Yapay zeka destekli onarım, ağaç görünümü, tablo görünümü, 12'den fazla programlama dilinde kod oluşturma, json'u csv, xml, yaml, özellikler ve daha fazlasıyla JSON verilerini biçimlendirin, görselleştirin, arayın ve değiştirin.
  * [KillBait API](https://killbait.com/api/doc) - KillBait API, kullanıcıların içerik değerlendirmesi için URL'ler göndermesine, potansiyel tıklama tuzaklarını tespit etmesine ve makaleleri kategorilere ayırmasına olanak tanır. API, saatte 1 gönderim ve günde 10 gönderim sınırıyla orta düzeyde yayınlama sıklığı için tasarlanmıştır. Medya iş ortakları daha yüksek limitler talep edebilir.
  * [Kreya](https://kreya.app) - gRPC API'lerini çağırmak ve test etmek için ücretsiz gRPC GUI istemcisi. GRPC API'lerini sunucu yansıması yoluyla içe aktarabilir.
  * [LoginLlama](https://loginllama.app) - Sahte ve şüpheli girişleri tespit etmek ve müşterilerinizi bilgilendirmek için bir giriş güvenliği API'si. Ayda 1.000 oturum açma işlemi için ücretsiz.
  * [Piyasa Verileri API'si](https://www.marketdata.app) - Hisse senetleri, opsiyonlar, yatırım fonları ve daha fazlası için gerçek zamanlı ve geçmişe dönük finansal veriler sağlar. Free Forever API katmanı, ücretsiz olarak 100 günlük API isteğine izin verir.
  * [Maxim AI](https://getmaxim.ai/) - Yapay zeka aracılarınızı simüle edin, değerlendirin ve gözlemleyin. Maxim, ekiplerin yapay zeka aracılarını güvenilir bir şekilde ve 5 kattan daha hızlı göndermesine yardımcı olan uçtan uca bir değerlendirme ve gözlemlenebilirlik platformudur. Bağımsız geliştiriciler ve küçük ekipler için sonsuza kadar ücretsiz (3 koltuk).
  * [microlink.io](https://microlink.io/) - Bir hizmet olarak herhangi bir web sitesini meta etiket normalleştirmesi, güzellik bağlantısı önizlemeleri, kazıma yetenekleri veya ekran görüntüleri gibi verilere dönüştürür. Günde 50 istek, her gün ücretsiz.
  * [Mintlify](https://mintlify.com) - API belgeleri için modern standart. Güzel ve bakımı kolay kullanıcı arayüzü bileşenleri, uygulama içi arama ve etkileşimli oyun alanı. 1 editör için ücretsiz.
  * [MockAPI](https://www.mockapi.io/) - MockAPI, hızlı bir şekilde API'ler oluşturmanıza, özel veriler oluşturmanıza ve RESTful arayüzünü kullanarak işlemler gerçekleştirmenize olanak tanıyan basit bir araçtır. MockAPI bir prototip oluşturma/test etme/öğrenme aracı olarak tasarlanmıştır. Bir proje/proje başına 2 kaynak ücretsiz.
  * [Mockerito](https://mockerito.com/) - 9 alanda (e-ticaret, finans, sağlık, eğitim, işe alım, sosyal medya, borsalar, hava durumu ve havacılık) gerçekçi veriler sağlayan ücretsiz sahte REST API hizmeti. Zorunlu kayıt yok, API anahtarı yok, sınırsız istek var. Ön uç prototipleme, API testi, web geliştirmeyi öğrenme ve öğretme için mükemmeldir.
  * [Mockfly](https://www.mockfly.dev/) - Mockfly, API taklit etme ve özellik bayrağı yönetimi için güvenilir bir geliştirme aracıdır. Sezgisel bir arayüzle sahte API'leri hızla oluşturun ve kontrol edin. Ücretsiz katman günde 500 istek sunar.
  * [Mocko.dev](https://mocko.dev/) - API'nizin proxy'sini kullanın, bulutta hangi uç noktaların taklit edileceğini seçin ve trafiği ücretsiz olarak denetleyin. Geliştirme ve entegrasyon testlerinizi hızlandırın.
  * [Çoklu Çıkış IP Adresi Denetleyicisi](https://ip.alstra.ca/) - Birden fazla düğümdeki çıkış IP adresinizi kontrol etmek ve IP'nizin farklı küresel bölge ve hizmetlere nasıl göründüğünü anlamak için ücretsiz ve basit bir araç. Control D gibi kural tabanlı DNS bölme araçlarını test etmek için kullanışlıdır.
  * [News API](https://newsapi.org) - Web'deki haberleri kodla arayın ve JSON sonuçlarını alın. Geliştiricilere her gün ücretsiz 100 sorgu sunulur. Makalelerde 24 saat gecikme var.
  * [numlookupapi.com](https://numlookupapi.com) - Ücretsiz telefon numarası doğrulama API'si - ayda 100 ücretsiz istek.
  * [OCR.Space](https://ocr.space/) - Bir OCR API'si, metin sonuçlarını JSON formatında döndüren resim ve pdf dosyalarını ayrıştırır. Ayda 25.000 istek ücretsizdir ve 1 MB dosya boyutu sınırı vardır.
  * [OpenAPI3 Designer](https://openapidesigner.com/) - Açık API 3 tanımlarını görsel olarak ücretsiz olarak oluşturun.
  * [Parseur](https://parseur.com) - Ayda 20 ücretsiz sayfa: PDF'lerden ve e-postalardan veri çıkarın. Yapay zeka destekli. Tam API erişimi.
  * [PDF-API.io](https://pdf-api.io) - PDF Otomasyon API'si, görsel şablon düzenleyici veya HTML'den PDF'ye, dinamik veri entegrasyonu ve bir API ile PDF oluşturma. Ücretsiz plan, ayda 100 PDF içeren bir şablonla birlikte gelir.
  * [PDFBolt](https://pdfbolt.com) - Gizlilik göz önünde bulundurularak tasarlanmış, geliştirici odaklı PDF oluşturma API'si. Stripe'tan ilham alan belgeler sunar ve ayda 500 ücretsiz PDF dönüşümü içerir.
  * [pdfEndpoint.com](https://pdfendpoint.com) - Basit bir API ile HTML veya URL'leri zahmetsizce PDF'ye dönüştürün. Ayda yüz dönüşüm ücretsiz.
  * [Pixela](https://pixe.la/) - Ücretsiz günlük veri tabanı hizmeti. Tüm işlemler API tarafından gerçekleştirilir. Isı haritaları ve çizgi grafiklerle görselleştirme de mümkündür.
  * [Postman](https://postman.com) - API geliştirmeye yönelik bir işbirliği platformu olan Postman ile iş akışlarını basitleştirin ve daha iyi API'leri daha hızlı oluşturun. Postacı Uygulamasını sonsuza kadar ücretsiz kullanın. Postman bulut özellikleri de belirli sınırlamalarla sonsuza kadar ücretsizdir.
  * [PrefectCloud](https://www.prefect.io/cloud/) - Veri akışı otomasyonu için eksiksiz bir platform. Ücretsiz plan, 5 dağıtılmış iş akışını ve ayda 500 dakikalık sunucusuz bilgi işlem kredisini içerir.
  * [Preset Cloud](https://preset.io/) - Barındırılan bir Apache Superset hizmeti. Sınırsız kontrol paneli ve grafikler, kodsuz bir grafik oluşturucu ve işbirliğine dayalı bir SQL düzenleyici içeren, en fazla 5 kişiden oluşan ekipler için sonsuza kadar ücretsiz.
  * [ProxySentry](https://proxysentry.io/) - Yerleşik proxy'leri ve VPN'leri algılayan IP API'si. ProxySentry.io, Rapidapi.com'da ayda 10 bin istekle ücretsiz bir katman sunuyor.
  * [Reducto](https://reducto.ai) - Yapılandırılmamış tüm belgeleri (PDF, XLSX, JPG, PPTX vb.) yapılandırılmış JSON verilerine dönüştürün. PDF formlarını ayrıştırın, çıkarın ve düzenleyin. 15.000 ücretsiz kredi ve kullandıkça öde ile ücretsiz katman.
  * [Rendi](https://rendi.dev) - FFmpeg API - FFmpeg için bir REST API'si, altyapıyı kullanmadan FFmpeg'i çevrimiçi çalıştırın. Aylık işlem kotası ve 4 vCPU'nun mevcut olduğu ücretsiz katman.
  * [RequestBin.com](https://requestbin.com) - HTTP isteklerini gönderebileceğiniz ücretsiz bir uç nokta oluşturun. Bu uç noktaya gönderilen tüm HTTP istekleri, ilgili yük ve başlıklarla birlikte kaydedilecektir; böylece web kancalarından ve diğer hizmetlerden gelen önerileri gözlemleyebilirsiniz.
  * [ROBOHASH](https://robohash.org/) - Herhangi bir metinden benzersiz ve harika görüntüler oluşturmaya yönelik web hizmeti.
  * [Scraper's Proxy](https://scrapersproxy.com) - Kazıma için basit HTTP proxy API'si. Kısıtlamalar, engellemeler veya captcha'lar konusunda endişelenmenize gerek kalmadan anonim olarak kazıyın. Javascript oluşturma dahil ayda ilk 100 başarılı not ücretsiz (destekle iletişime geçerseniz daha fazlasını alabilirsiniz).
  * [ScrapingAnt](https://scrapingant.com/) - Başsız Chrome kazıma API'si ve ücretsiz kontrol edilen proxy'ler hizmeti. Javascript oluşturma, premium dönüşümlü proxy'ler, CAPTCHA'lardan kaçınma. Ücretsiz 10.000 API kredisi.
  * [SerpApi](https://serpapi.com/) - Gerçek zamanlı arama motoru kazıma API'si. Google, YouTube, Bing, Baidu, Walmart ve diğer birçok makine için yapılandırılmış JSON sonuçlarını döndürür. Ücretsiz plan ayda 100 başarılı API çağrısını içerir.
  * [Sheetson](https://sheetson.com) - Tüm Google E-Tablolarını anında bir RESTful API'sine dönüştürün. Sayfa başına 1.000 ücretsiz satır içeren ücretsiz plan mevcuttur.
  * [SikkerAPI](https://sikkerapi.com) - Ücretsiz IP İtibarı ve Tehdit İstihbaratı, küresel olarak dağıtılmış yüksek etkileşimli bal küpü ağı ve topluluk tarafından rapor edilen kötüye kullanım olayları tarafından desteklenmektedir. Günde 1.000 ücretsiz IP araması, TAXII göstergesi ve raporu, kara listelerimizden günlük 5.000 yeni IP çekin ve kendi CIDR aralıklarınızı (/16) ücretsiz olarak izleyin.
  * [Simplescraper](https://simplescraper.io) - Her işlemden sonra web kancanızı tetikleyin. Ücretsiz plan 100 bulut kazıma kredisi içerir.
  * [Geekflare API](https://geekflare.com/api/) - Geekflare API, web sitelerini Markdown'a aktarmanıza, ekran görüntüleri almanıza, TLS taramaları ve DNS aramaları gerçekleştirmenize, yükleme sürelerini test etmenize ve daha pek çok şeye olanak tanır. Ücretsiz plan ayda 500 API kredisi sunar (ör. 500 DNS araması, 250 web notu veya 100 ekran görüntüsü). Bkz. [kredi eşleme](https://docs.geekflare.com/api/api-credit-mapping).
  * [SmartParse](https://smartparse.io) - SmartParse, zamandan ve maliyetten tasarruf sağlayan geliştirici araçları sunan, API platformuna bir veri taşıma ve CSV'dir. Ücretsiz katman ayda 300 İşlem Birimi, Tarayıcı yüklemeleri, Veri karantinaya alma, Devre kesiciler ve İş Uyarılarını içerir.
  * [Sofodata](https://www.sofodata.com/) - CSV dosyalarından güvenli RESTful API'ler oluşturun. Bir CSV dosyası yükleyin ve daha hızlı uygulama geliştirme olanağı sağlayan API aracılığıyla verilere anında erişin. Ücretsiz plan ayda 2 API ve 2.500 API çağrısı içerir. Kredi kartına ihtiyacınız yok.
  * [Sqlable](https://sqlable.com/) - SQL formatlayıcı ve doğrulayıcı, SQL regex test cihazı, sahte veri oluşturucu ve etkileşimli veritabanı oyun alanları dahil olmak üzere ücretsiz çevrimiçi SQL araçlarından oluşan bir koleksiyon.
  * [Supportivekoala](https://supportivekoala.com/) - Şablonlar aracılığıyla girişinize göre görüntüleri otomatik olarak oluşturmanıza olanak tanır. Ücretsiz plan ayda 50'ye kadar görsel oluşturmanıza olanak tanır.
  * [Svix](https://www.svix.com/) - Hizmet olarak Web Kancaları. Ayda 50.000'e kadar mesaja kadar ücretsiz gönderin.
  * [Tavily AI](https://tavily.com/) - Araştırma sonuçlarını düzenleme becerisine sahip, çevrimiçi arama, hızlı öngörüler ve kapsamlı araştırmalar için API. Ücretsiz katman için kredi kartı gerekmeden ayda 1000 istek.
  * [TemplateFox](https://pdftemplateapi.com) - Görsel şablon düzenleyici, dinamik veri birleştirme ve 7 dil için SDK'lar içeren PDF oluşturma API'si. Ücretsiz plan ayda 60 PDF ve 3 şablon içerir.
  * [IP API](https://theipapi.com/) - Günde 1000 ücretsiz istek içeren IP Coğrafi Konum API'si. Ülke, şehir, bölge ve daha fazlasını içeren bir IP adresinin konumu hakkında bilgi sağlar.
  * [TinyMCE](https://www.tiny.cloud) - zengin metin düzenleme API'si. Temel özellikler sınırsız kullanım için ücretsizdir.
  * [Tomorrow.io Hava Durumu API'si](https://www.tomorrow.io/weather-api/) - Ücretsiz hava durumu API planı sunar. Küresel kapsama alanı, geçmiş veriler ve hava durumu izleme çözümleriyle doğru ve güncel hava durumu tahminleri sağlar.
  * [Treblle](https://www.treblle.com) - Treblle, ekiplerin API'leri oluşturmasına, göndermesine ve yönetmesine yardımcı olur. Gelişmiş API günlük toplama, gözlemlenebilirlik, belgeler ve hata ayıklama özellikleriyle. Tüm özelliklere ücretsiz olarak sahip olursunuz ancak ücretsiz katmanda ayda 250.000'e kadar istek sınırı vardır.
  * [UniRateAPI](https://unirateapi.com) - 590'dan fazla para birimi ve kripto için gerçek zamanlı döviz kurları. Ücretsiz plandaki sınırsız API çağrıları, geliştiriciler ve finans uygulamaları için mükemmeldir.
  * [vatcheckapi.com](https://vatcheckapi.com) - Basit ve ücretsiz KDV numarası doğrulama API'si. Ayda 150 ücretsiz doğrulama.
  * [WeatherXu](https://weatherxu.com/) - API'mız aracılığıyla mevcut koşulları, saatlik ve günlük tahminleri ve hava durumu uyarılarını içeren küresel hava durumu verileri. Gelişmiş tahmin doğruluğu sağlamak amacıyla birden fazla hava durumu modelini analiz etmek ve birleştirmek için AI modellerini ve ML sistemlerini entegre etme. Ücretsiz katman ayda 10.000 API çağrısını içerir.
  * [WebScraping.AI](https://webscraping.ai) - Yerleşik ayrıştırma, Chrome oluşturma ve proxy'lere sahip Basit Web Scraping API'si. Ayda iki bin ücretsiz API çağrısı.
  * [Ağırlıklar ve Önyargılar](https://wandb.ai) - Geliştiricinin ilk MLOps platformu. Deneme izleme, veri kümesi sürüm oluşturma ve model yönetimi ile daha iyi modelleri daha hızlı oluşturun. Yalnızca kişisel projelere yönelik ücretsiz katman; 100 GB depolama alanı dahildir.
  * [IP'm Nedir](https://whatismyip.help) - Otomasyon, komut dosyaları ve ağ sorun giderme için farklı çıktı biçimlerine sahip bir API aracılığıyla genel IPv4 ve IPv6 adresinizi ve ilgili istek verilerinizi kontrol etmenizi sağlayan ücretsiz bir hizmet.
  * [What The Diff](https://whatthediff.ai) - Yapay zeka destekli kod inceleme asistanı. Ücretsiz planın aylık 25.000 token (~10 PR) sınırı vardır.
  * [wolfram.com](https://wolfram.com/language/) - Bulutta yerleşik, bilgiye dayalı algoritmalar.
  * [wrapapi.com](https://wrapapi.com/) - Herhangi bir web sitesini parametreli bir API'ye dönüştürün. Ayda 30 bin API çağrısı.
  * [Zenscrape](https://zenscrape.com/web-scraping-api) - Başsız tarayıcılar, konut IP'leri ve basit fiyatlandırma ile Web kazıma API'si. Öğrenciler ve kar amacı gütmeyen kuruluşlar için ayda bin adet ücretsiz API çağrısı ve ekstra kredi.
  * [Zipcodebase](https://zipcodebase.com) - Ücretsiz Posta Kodu API'si, Dünya Çapındaki Posta Kodu Verilerine erişim. Aylık 5.000 ücretsiz istek.
  * [Zipcodestack](https://zipcodestack.com) - Ücretsiz Posta Kodu API'si ve Posta Kodu Doğrulaması. Ayda on bin ücretsiz istek.
  * [Zuplo](https://zuplo.com/) - API'leri Edge'e tasarlamak, oluşturmak ve dağıtmak için ücretsiz API Yönetim platformu. Herhangi bir API'ye birkaç dakika içinde API Anahtarı kimlik doğrulaması, hız sınırlaması, geliştirici belgeleri ve Para Kazanma ekleyin. OpenAPI'de yereldir ve web standardı apis ve Typescript ile tamamen programlanabilir. Ücretsiz plan, 10'a kadar proje, sınırsız üretim ortamı, aylık 1 milyon istek ve 10 GB çıkış sunar.

**[⬆️Başa Dön](#table-of-contents)**

## Artifact Repos

  * [Gemfury](https://gemfury.com) - Maven, PyPi, NPM, Go Module, Nuget, APT ve RPM depoları için özel ve genel yapı depoları. Kamu projeleri için ücretsiz.
  * [jitpack.io](https://jitpack.io/) - GitHub'daki JVM ve Android projeleri için Maven deposu, genel projeler için ücretsiz.
  * [paperspace](https://www.paperspace.com/) - Yapay zeka modelleri oluşturun ve ölçeklendirin, Yapay zeka uygulamaları geliştirin, eğitin ve dağıtın, ücretsiz plan: genel projeler, 5 Gb depolama, temel örnekler.
  * [RepoFlow](https://repoflow.io) - RepoFlow Npm, PyPI, Docker, Go, Helm ve daha fazlasının desteğiyle paket yönetimini basitleştirir. 10 GB depolama alanı, 10 GB bant genişliği, 100 paket ve bulutta sınırsız kullanıcı veya yalnızca kişisel kullanım için kendi kendine barındırılan özelliklerle ücretsiz deneyin.
  * [RepoForge](https://repoforge.io) - Python, Debian, NPM paketleri ve Docker kayıtları için bulutta barındırılan özel depo. Açık kaynak/kamuya açık projeler için ücretsiz plan.
  * [repsy.io](https://repsy.io) - 1 GB Ücretsiz özel/genel Maven Deposu.

**[⬆️Başa Dön](#table-of-contents)**

## Tools for Teams and Collaboration

  * [3Cols](https://3cols.com/) - Kişisel ve ortak kod için ücretsiz, bulut tabanlı bir kod pasajı yöneticisi.
  * [BookmarkOS.com](https://bookmarkos.com) - Klasör işbirliğiyle özelleştirilebilir bir çevrimiçi masaüstünde ücretsiz hepsi bir arada yer işareti yöneticisi, sekme yöneticisi ve görev yöneticisi.
  * [Braid](https://www.braidchat.com/) - Ekipler için tasarlanmış sohbet uygulaması. Genel erişim grubu, sınırsız kullanıcı, geçmiş ve entegrasyonlar için ücretsiz. ayrıca kendi kendine barındırılabilen açık kaynaklı bir sürüm sağlar.
  * [Calendly](https://calendly.com) - Calendly, toplantıları bağlamak ve planlamak için kullanılan bir araçtır. Ücretsiz plan, kullanıcı başına 1 Takvim bağlantısı ve Sınırsız oturum sağlar. Masaüstü ve Mobil uygulamalar da sunulmaktadır.
  * [cally.com](https://cally.com/) - Bir toplantı için mükemmel saati ve tarihi bulun. Kullanımı basit, küçük ve büyük gruplar için harika çalışıyor.
  * [cDox](https://cdox.ca) - Kanada'da barındırılan özel belge düzenleyici. Temiz, herkese açık bağlantılara sahip belgeler yazın, biçimlendirin, işbirliği yapın ve yayınlayın. Veriler hiçbir zaman yapay zeka eğitimi için kullanılmaz. Ücretsiz plan 50 MB depolama alanı, 3 adede kadar genel bağlantı ve PDF, Word ve Markdown'a aktarma içerir.
  * [Chanty.com](https://chanty.com/) - Chanty, Slack'in başka bir alternatifidir. Sınırsız genel ve özel görüşme, aranabilir geçmiş, sınırsız 1:1 sesli çağrı, sınırsız sesli mesaj, on entegrasyon ve ekip başına 20 GB depolama alanıyla küçük ekipler (10'a kadar) için sonsuza kadar ücretsiz bir plana sahiptir.
  * [DevToolLab](https://devtoollab.com) - Araç başına bir girişi otomatik olarak kaydetme yeteneği, standart işlem hızı ve topluluk desteği ile tüm temel araçlara ücretsiz erişim sunan çevrimiçi geliştirici araçları.
  * [Discord](https://discord.com/) - Herkese açık/özel odalarla sohbet edin. Metin, ses, video ve ekran paylaşımı yeteneklerini işaretleyin. Sınırsız kullanıcı için ücretsizdir.
  * [Dubble](https://dubble.so/) - Ücretsiz Adım Adım Kılavuz yaratıcısı. Ekran görüntüleri alın, süreçleri belgeleyin ve ekibinizle işbirliği yapın. Ayrıca eşzamansız ekran kaydını da destekler.
  * [Duckly](https://duckly.com/) - Ekibinizle gerçek zamanlı olarak konuşun ve işbirliği yapın. Programlamayı IDE, terminal paylaşımı, ses, video ve ekran paylaşımıyla eşleştirin. Küçük takımlar için ücretsiz.
  * [element.io](https://element.io/) - Matrix üzerine kurulu, merkezi olmayan ve açık kaynaklı bir iletişim aracı. Grup sohbetleri, doğrudan mesajlaşma, şifreli dosya aktarımları, sesli ve görüntülü sohbetler ve diğer servislerle kolay entegrasyon.
  * [evernote.com](https://evernote.com/) - Bilgileri düzenlemeye yönelik araç. Notlarınızı paylaşın ve başkalarıyla birlikte çalışın
  * [Fibery](https://fibery.io/) - Bağlantılı çalışma alanı platformu. Tek kullanıcılar için ücretsiz, 2 GB'a kadar disk alanı.
  * [Fibo](https://fibo.dev) - Çevik ekiplere yönelik, sınırsız sayıda üyenin daha hızlı planlama için hikaye puanlarını tahmin etmesine olanak tanıyan ücretsiz bir çevrimiçi gerçek zamanlı scrum poker aracı.
  * [Fizzy](https://www.fizzy.do/) - Proje yönetimi ve sorun takibi için Kanban tabanlı platform. Herkese açık panolar oluşturun, web kancaları kurun, kart damgalama kullanın ve sınırsız kullanıcıyı takip edin - 1000 öğeye kadar ücretsiz.
  * [flat.social](https://flat.social) - Ekip toplantıları ve mutlu saatler sosyalleri için etkileşimli, özelleştirilebilir alanlar. Sınırsız toplantı, 8 eşzamanlı kullanıcıya kadar ücretsiz.
  * [flock.com](https://flock.com) - Ekibinizin iletişim kurmasının daha hızlı bir yolu. Ücretsiz Sınırsız Mesaj, Kanal, Kullanıcı, Uygulama ve Entegrasyon
  * [GitBook](https://www.gitbook.com/) - Ürün belgelerinden dahili bilgi tabanlarına ve API'lere kadar teknik bilginin toplanması ve belgelenmesi için platform. Bireysel geliştiriciler için ücretsiz plan.
  * [GitDailies](https://gitdailies.com) - Ekibinizin GitHub'daki Taahhüt ve Çekme İsteği etkinliğinin günlük raporları. Push görselleştiricisi, eş tanıma sistemi ve özel uyarı oluşturucuyu içerir. Ücretsiz katmanda sınırsız kullanıcı, üç depo ve 3 uyarı yapılandırması bulunur.
  * [gitter.im](https://gitter.im/) - GitHub için sohbet edin. Sınırsız genel ve özel odalar, 25 kişiye kadar ekipler için ücretsiz
  * [gokanban.io](https://gokanban.io) - Söz dizimi tabanlı, hızlı kullanım için kayıt gerektirmeyen Kanban Kurulu. Hiçbir sınırlama olmadan ücretsiz.
  * [Hackmd.io](https://hackmd.io/) - Markdown formatındaki belgeler/dosyalar için gerçek zamanlı işbirliği ve yazma aracı. Google Dokümanlar gibi ancak işaretleme dosyaları için. Ücretsiz sınırsız sayıda "not", ancak özel notlar ve şablon için ortak çalışan (davetli) sayısı [sınırlı olacaktır](https://hackmd.io/pricing).
  * [HeySpace](https://hey.space) - Sohbet, takvim, zaman çizelgesi ve video görüşmeleri içeren görev yönetimi aracı. 5 kullanıcıya kadar ücretsizdir.
  * [Huly](https://huly.io/) - Hepsi Bir Arada Proje Yönetim Platformu (Linear, Jira, Slack, Notion, Motion'a alternatif) - sınırsız kullanıcı, çalışma alanı başına 10 GB depolama, 10 GB video(ses) trafiği.
  * [Keybase](https://keybase.io/) - Keybase, Slack'e bir FOSS alternatifidir; ailelerden topluluklara ve şirketlere kadar herkesin sohbetlerini ve dosyalarını güvende tutar.
  * [Linkinize](https://linkinize.com) - Etiketleme, çoklu çalışma alanları ve ortak çalışmaya sahip ekipler için yer işareti yöneticisi. Ücretsiz planda 4 çalışma alanı ve 10 ekip üyesi bulunur.
  * [Lockitbot](https://www.lockitbot.com/) - Slack içindeki Odalar, Geliştirme ortamları, sunucular vb. gibi paylaşılan kaynakları ayırın ve kilitleyin. 2 kaynağa kadar ücretsiz
  * [meet.jit.si](https://meet.jit.si/) - Tek tıkla görüntülü konuşmalar ve ücretsiz ekran paylaşımı
  * [Miro](https://miro.com/) - Dağıtılmış ekipler için ölçeklenebilir, güvenli, cihazlar arası ve kurumsal kullanıma hazır işbirliği beyaz tahtası. Ücretsiz bir planla.
  * [Notion](https://www.notion.so/) - Notion, görevleri, wiki'leri ve veritabanlarını entegre eden işaretleme desteğine sahip bir not alma ve işbirliği uygulamasıdır. Şirket, uygulamayı not alma, proje yönetimi ve görev yönetimi için hepsi bir arada bir çalışma alanı olarak tanımlıyor. Çapraz platform uygulamalarına ek olarak çoğu web tarayıcısından da erişilebilir.
  * [Nuclino](https://www.nuclino.com) - Ekibinizin tüm bilgileri, dokümanları ve notları için hafif ve ortak çalışmaya dayalı bir wiki. Tüm temel özellikleri, 50'ye kadar öğeyi ve 5 GB depolama alanını içeren ücretsiz plan.
  * [OnlineInterview.io](https://onlineinterview.io/) - Yerleşik görüntülü sohbet, çizim tahtası ve kodunuzu tarayıcıda derleyip çalıştırabileceğiniz çevrimiçi kod düzenleyiciye sahip ücretsiz kod röportaj platformu. Tek tıklamayla uzaktan görüşme odası oluşturabilirsiniz.
  * [paste.sh](https://paste.sh/) - Bu bir JavaScript ve Kripto tabanlı basit yapıştırma sitesidir.
  * [Pastefy](https://pastefy.app/) - İsteğe bağlı İstemci Şifrelemesi, Çoklu Sekme Yapıştırmaları, API, vurgulanmış Düzenleyici ve daha fazlasını içeren güzel ve basit Pastebin.
  * [Pendulums](https://pendulums.io/) - Pendulums, kullanımı kolay arayüzü ve değerli istatistikleriyle zamanınızı daha iyi yönetmenize yardımcı olan bir boş zaman izleme aracıdır.
  * [Proton Pass](https://proton.me/pass) - Yerleşik e-posta takma adlarına, 2FA kimlik doğrulayıcısına, paylaşıma ve geçiş anahtarlarına sahip şifre yöneticisi. Web'de, tarayıcı uzantısında, mobil uygulamada ve masaüstünde kullanılabilir.
  * [Pullflow](https://pullflow.com) - Pullflow, GitHub, Slack ve VS Code genelinde kod inceleme iş birliği için yapay zekayla geliştirilmiş bir platform sunar.
  * [Pumble](https://pumble.com) - Ücretsiz takım sohbeti uygulaması. Sınırsız kullanıcı ve mesaj geçmişi, sonsuza kadar ücretsiz.
  * [Quidlo Zaman Çizelgeleri](https://www.quidlo.com/timesheets) - Ekipler için basit bir zaman çizelgesi ve zaman izleme uygulaması. Ücretsiz plan, 10 kullanıcıya kadar zaman izleme ve rapor oluşturma özelliklerine sahiptir.
  * [Raindrop.io](https://raindrop.io) - MacOS, Windows, Android, iOS ve Web için özel ve güvenli yer işareti koyma uygulaması. Ücretsiz Sınırsız Yer İmleri ve İşbirliği.
  * [Revolt.chat](https://revolt.chat/) - Gizliliğinize saygı duyan[Discord](https://discord.com/) için bir Açık Kaynak alternatifi. Ayrıca discord'a ait çoğu özel özelliğe ücretsiz olarak sahiptir. Revolt, güvenli ve hızlı, aynı zamanda %100 ücretsiz, hepsi bir arada bir uygulamadır. her özellik ücretsizdir. Ayrıca, çoğu ana sohbet uygulamasının aksine (resmi ve resmi olmayan) eklenti desteğine sahiptirler.
  * [Rocket.Chat](https://rocket.chat/) - Çok Kanallı özelliklere, Matrix Federasyonuna, diğer uygulamalarla Bridge'e, Sınırsız mesajlaşmaya ve Tam mesajlaşma geçmişine sahip açık kaynaklı iletişim platformu.
  * [ruttl.com](https://ruttl.com/) - Dijital geri bildirim toplamak ve web sitelerini, PDF'leri ve görselleri incelemek için en iyi hepsi bir arada geri bildirim aracı.
  * [Tarayıcı Üzerinden Ekran Paylaşımı](https://screensharing.net) - Ücretsiz ekran paylaşım aracı, ekranınızı doğrudan tarayıcınızdan ortak çalışanlarla paylaşın, indirme veya kayıt gerekmez. Ücretsiz.
  * [seafile.com](https://www.seafile.com/) - Özel veya bulut depolama, dosya paylaşımı, senkronizasyon, tartışmalar. Bulut sürümünde yalnızca 1 GB yer var
  * [SiteDots](https://sitedots.com/) - Web sitesi projeleri için geri bildirimleri doğrudan web sitenizde paylaşın; öykünme, tuval veya geçici çözüm olmadan. Tamamen işlevsel ücretsiz katman.
  * [Slab](https://slab.com/) - Ekipler için modern bir bilgi yönetimi hizmeti. 10 kullanıcıya kadar ücretsizdir.
  * [slack.com](https://slack.com/) - Bazı özellik sınırlamalarıyla sınırsız kullanıcı için ücretsiz
  * [StatusPile](https://www.statuspile.com/) - Durum sayfalarının durum sayfası. Yukarı akış sağlayıcılarınızın durum sayfalarını takip edebilir misiniz?
  * [Stickies](https://stickies.app/) - Beyin fırtınası, içerik iyileştirme ve notlar için kullanılan görsel işbirliği uygulaması. 3 Duvara kadar ücretsiz, sınırsız kullanıcı ve 1 GB depolama alanı.
  * [StreamBackdrops](https://streambackdrops.com) - Görüntülü görüşmeler ve ekip toplantıları için ücretsiz HD sanal arka planlar. Zoom, Teams ve Google Meet için profesyonel arka planlar. Kayıt olmanıza gerek yok, kişisel kullanım için ücretsiz.
  * [talky.io](https://talky.io/) - Ücretsiz grup görüntülü sohbeti. Anonim. Eşler arası. Eklenti, kayıt veya ödeme gerekmez
  * [Teamcamp](https://www.teamcamp.app) - Yazılım geliştirme şirketleri için hepsi bir arada proje yönetimi uygulaması.
  * [Takımlık](https://teamhood.com/) - Ücretsiz Proje, Görev ve Sorun izleme yazılımı. Kanban'ı Swimlanes ve tam Scrum uygulamasıyla destekler. Entegre zaman takibine sahiptir. Beş kullanıcı ve üç proje portföyü için ücretsiz.
  * [Teamplify](https://teamplify.com) - Team Analytics ve Smart Daily Standup ile ekip geliştirme süreçlerini iyileştirin. Önce uzaktan çalışan ekipler için tam özellikli İzin Süresi yönetimini içerir. 5 kullanıcıya kadar küçük gruplar için ücretsizdir.
  * [Telegram](https://telegram.org/) - Telegram hızlı, güvenilir mesajlaşma ve çağrı isteyen herkes içindir. İş kullanıcıları ve küçük ekipler büyük grupları, kullanıcı adlarını, masaüstü uygulamalarını ve güçlü dosya paylaşım seçeneklerini beğenebilir.
  * [Tencent RTC](https://trtc.io/) - Tencent Gerçek Zamanlı İletişim (TRTC), grup sesli/görüntülü aramalar için çözümler sunar. İlk yıl için ayda 10.000 ücretsiz dakika.
  * [TimeCamp](https://www.timecamp.com/) - Sınırsız kullanıcı için ücretsiz zaman izleme yazılımı. Jira, Trello, Asana vb. PM araçlarıyla kolayca entegre olur.
  * [tldraw.com](https://tldraw.com) - Akıllı oklar, yakalama, yapışkan notlar ve SVG dışa aktarma özelliklerine sahip ücretsiz açık kaynaklı beyaz tahta ve diyagram oluşturma aracı. İşbirliğine dayalı düzenleme için çok oyunculu mod. Ücretsiz resmi VS Code uzantısı da mevcuttur.
  * [transfernow](https://www.transfernow.net/) - dosyaları aktarmak ve paylaşmak için en basit, en hızlı ve en güvenli arayüz. Fotoğrafları, videoları ve diğer büyük dosyaları zorunlu bir abonelik olmadan gönderin.
  * [Römorkör](https://tugboat.qa) - Otomatik ve isteğe bağlı olarak her çekme isteğinin ön izlemesini yapın. Herkes için ücretsiz, kâr amacı gütmeyen kuruluşlar için ücretsiz Nano katmanı.
  * [twist.com](https://twist.com) - Konuşmaların düzenli ve konuyla ilgili kaldığı, eşzamansız, uyumlu bir ekip iletişim uygulaması. Ücretsiz ve Sınırsız planlar mevcuttur. Uygun takımlara indirim sağlanır.
  * [userforge.com](https://userforge.com/) - Birbirine bağlı çevrimiçi kişiler, kullanıcı hikayeleri ve bağlam haritalaması.  En fazla 3 kişi ve iki ortak çalışan için tasarım ve geliştirmeyi senkronize halde tutmaya yardımcı olur.
  * [Görsel Hata Ayıklama](https://visualdebug.com) - Daha iyi müşteri-geliştirici iletişimi için görsel bir geri bildirim aracı
  * [Webex](https://www.webex.com/) - 100 katılımcıyla toplantı başına 40 dakika sunan ücretsiz planlı görüntülü toplantılar.
  * [Webvizio](https://webvizio.com) - Doğrudan canlı web siteleri ve web uygulamaları, resimler, PDF'ler ve tasarım dosyaları üzerindeki görevlerde web geliştirme işbirliğini kolaylaştırmak için web sitesi geri bildirim aracı, web sitesi inceleme yazılımı ve hata raporlama aracı.
  * [whereby.com](https://whereby.com/) - Tek tıklamayla ücretsiz görüntülü konuşmalar (eski adıyla Görünen.in)
  * [windmill.dev](https://windmill.dev/) - Windmill, minimum Python ve Typescript komut dosyalarıyla üretim düzeyinde çok adımlı otomasyonu ve dahili uygulamaları hızla oluşturmaya yönelik açık kaynaklı bir geliştirici platformudur. Ücretsiz kullanıcı olarak en fazla üç premium olmayan çalışma alanı oluşturabilir ve bunlara üye olabilirsiniz.
  * [wistia.com](https://wistia.com/) - Ziyaretçilerinizi, 25 videoyu ve Wistia markalı oynatıcıyı anlamanıza yardımcı olacak izleyici analizleri, HD video sunumu ve pazarlama araçlarıyla video barındırma
  * [wormhol.org](https://www.wormhol.org/) - Kolay dosya paylaşım hizmeti. 5 GB'a kadar sınırsız dosyayı istediğiniz sayıda eşle paylaşın.
  * [Solucan deliği](https://wormhole.app/) - 24 saate kadar uçtan uca şifrelemeyle 5 GB'a kadar dosyaları paylaşın. 5 GB'tan büyük dosyalar için, dosyalarınızı doğrudan göndermek üzere eşler arası aktarımı kullanır.
  * [zoom.us](https://zoom.us/) - Güvenli Video ve Web konferansı eklentileri mevcut. Ücretsiz plan 40 dakika ile sınırlıdır.
  * [Zulip](https://zulip.com/) - Benzersiz bir e-posta benzeri ileti dizisi modeliyle gerçek zamanlı sohbet. Ücretsiz plan, 10.000 arama geçmişi mesajı ve 5 GB'a kadar Dosya depolama alanı içerir. ayrıca kendi kendine barındırılabilen açık kaynaklı bir sürüm sağlar.
  * [RightFeature](https://rightfeature.com/) - Müşterilerinizden kolayca geri bildirim toplayın, müşteri geri bildirimlerini ürün yol haritanıza dönüştürün. Kullanıcılarınız için gerçekten önemli olan özellikleri toplayın, önceliklendirin ve gönderin.

**[⬆️Başa Dön](#table-of-contents)**

## CMS

  * [İçerikli](https://www.contentful.com/) - Başsız CMS. Buluttaki içerik yönetimi ve dağıtım API'leri. Beş kullanıcı, 25.000 kayıt, 48 İçerik Türü, 2 yerel ayar içeren bir ücretsiz Topluluk alanıyla birlikte gelir.
  * [Kozmik](https://www.cosmicjs.com/) - Başsız CMS ve API araç seti. Geliştiriciler için ücretsiz kişisel planlar.
  * [Kristalleştir](https://crystallize.com) - E-ticaret desteğiyle Başsız PIM. Yerleşik GraphQL API'si. Ücretsiz sürüm sınırsız kullanıcı, 1000 katalog öğesi, 5 GB/ay bant genişliği ve 25 bin/ay API çağrısı içerir.
  * [DatoCMS](https://www.datocms.com/) - Küçük projeler için ücretsiz katman sunar. DatoCMS, GraphQL tabanlı bir CMS'dir. Alt kademede ayda 100 bin çağrınız var.
  * [Hygraph](https://hygraph.com/) - Küçük projeler için ücretsiz katman sunar. GraphQL'in ilk API'si. Eski çözümlerden GraphQL yerel Headless CMS'ye geçin ve önce çok kanallı içerik API'sini sunun.
  * [Prizmik](https://www.prismic.io/) - Başsız CMS. Tamamen barındırılan ve ölçeklenebilir API'ye sahip içerik yönetimi arayüzü. Topluluk Planı, bir kullanıcıya sınırsız API çağrıları, belgeler, özel türler, varlıklar ve yerel ayarlar sağlar. Bir sonraki projeniz için ihtiyacınız olan her şey. Açık İçerik/Açık Kaynak projeleri için daha büyük ücretsiz planlar mevcuttur.
  * [Sanity.io](https://www.sanity.io/) - Açık kaynaklı bir düzenleme ortamına ve gerçek zamanlı olarak barındırılan bir veri deposuna sahip yapılandırılmış içerik platformu. Sınırsız proje. Sınırsız yönetici kullanıcı, yönetici olmayan üç kullanıcı, iki veri kümesi, 500.000 API CDN isteği, 10 GB bant genişliği ve proje başına ücretsiz olarak 5 GB varlık dahildir.
  * [Solo](https://soloist.ai) - Mozilla'dan ücretsiz AI web sitesi yaratıcısı, birkaç basit girdiyle işletmeniz için güzel bir web sitesi oluşturun. Ücretsiz özel alan adı, kredi kartına gerek yok.
  * [Squidex](https://squidex.io/) - Küçük projeler için ücretsiz katman sunar. Önce API/GraphQL. Açık kaynaktır ve olay kaynağına dayalıdır (her değişikliği otomatik olarak gerçekleştirir).
  * [Storyblok](https://www.storyblok.com) - Geliştiriciler ve pazarlamacılar için tüm modern çerçevelerle çalışan, Başsız bir CMS. Topluluk (ücretsiz) katmanı; Yönetim API'si, Görsel Düzenleyici, on kaynak, Özel Alan Türleri, Uluslararasılaştırma (sınırsız dil/yerel ayarlar), Varlık Yöneticisi (2500'e kadar varlık), Görüntü Optimize Etme Hizmeti, Arama Sorgusu, Web Kancası + 250 GB Trafik/ay dahil sunar.
  * [TinaCMS](https://tina.io/) - Forestry.io'nun değiştirilmesi. Markdown, MDX ve JSON'u destekleyen açık kaynaklı Git destekli başsız CMS. Temel teklif, iki kullanıcı mevcut olduğunda ücretsizdir.
  * [WPJack](https://wpjack.com) - WordPress'i herhangi bir bulutta 5 dakikadan kısa sürede kurun! Ücretsiz katmanda 1 sunucu, 2 site, ücretsiz SSL sertifikaları ve sınırsız cron işleri bulunur. Süre sınırı veya son kullanma tarihi yok; web siteniz, sizin yönteminiz.

**[⬆️Başa Dön](#table-of-contents)**

## Code Generation

* [Appinvento](https://appinvento.io/) - Ücretsiz, kodsuz bir uygulama oluşturucu. Otomatik olarak oluşturulan arka uç kaynak koduna tam erişim sağlar ve sınırsız API'lere ve rotalara izin verir. Ücretsiz planda üç proje ve beş tablo yer alıyor.
* [DhiWise](https://www.dhiwise.com/) - Figma tasarımlarını dinamik Flutter ve React uygulamalarına dönüştürür. Kod oluşturma teknolojisi, üretime hazır mobil ve web deneyimleri oluşturmak için iş akışlarını optimize etmek üzere tasarlanmıştır.
* [Karbon Sites](https://www.karbonsites.space) - Metin istemlerinden, taslaklardan veya özgeçmişlerden üretime hazır ön uç kodu üreten, yapay zeka destekli bir site oluşturucu ve düzenleyici. Özellikler arasında yerel Android (APK) dışa aktarımı ve ayda 5 nesil içeren ücretsiz bir katman (özel Gemini API anahtarıyla sınırsız) yer alır.
* [Metalama](https://www.postsharp.net/metalama) - Kaynak kodunu temiz tutmak için derleme sırasında anında standart kod üreten, C#'a özgü bir araç. Açık kaynaklı projeler için ücretsizdir; ticari dostu ücretsiz katmanı en fazla üç özelliği içerir.
* [Supermaven](https://www.supermaven.com/) - VS Code, JetBrains ve Neovim için yüksek hızlı bir AI kod tamamlama eklentisi. Ücretsiz katman, ultra düşük gecikme süresine odaklanarak sınırsız satır içi tamamlama sağlar.
* [v0.dev](https://v0.dev/) - Vercel tarafından oluşturulan v0, shadcn/ui ve Tailwind CSS'yi kullanarak kopyala ve yapıştır dostu React kodu oluşturur. Aylık 1.200 başlangıç ​​kredisi ve 200 ücretsiz kredi sağlayan bir kredi sistemi kullanır.

**[⬆️Başa Dön](#table-of-contents)**

## Code Quality

  * [beanstalkapp.com](https://beanstalkapp.com/) - Kod yazmak, incelemek ve dağıtmak için eksiksiz bir iş akışı), bir kullanıcı için ücretsiz hesap ve 100 MB depolama alanına sahip bir depo
  * [codacy.com](https://www.codacy.com/) - PHP, Python, Ruby, Java, JavaScript, Scala, CSS ve CoffeeScript için otomatik kod incelemeleri; sınırsız genel ve özel depolar için ücretsiz
  * [Codeac.io](https://www.codeac.io/infrastructure-as-code.html?ref=free-for-dev) - DevOps için Kod inceleme aracı olarak Otomatik Altyapı GitHub, Bitbucket ve GitLab (hatta kendi kendine barındırılan) ile entegre olur. Standart dillerin yanı sıra Ansible, Terraform, CloudFormation, Kubernetes ve daha fazlasını da analiz eder. (açık kaynak ücretsiz)
  * [codecov.io](https://codecov.io/) - Kod kapsamı aracı (SaaS), Açık Kaynak için ücretsiz ve bir ücretsiz özel depo
  * [CodeFactor](https://www.codefactor.io) - Git için Otomatik Kod İncelemesi. Ücretsiz sürümde sınırsız kullanıcı, halka açık depolar ve bir özel depo bulunur.
  * [coderabbit.ai](https://coderabbit.ai) - GitHub/GitLab ile entegre olan, yapay zeka destekli kod inceleme aracı. Ücretsiz katman, saatte 200 dosya, saatte 3 inceleme ve saatte 50 görüşme içerir. Açık kaynaklı projeler için sonsuza kadar ücretsiz.
  * [CodSpeed](https://codspeed.io) - CI ardışık düzenlerinizde performans takibini otomatikleştirin. Kesin ve tutarlı ölçümler sayesinde performans gerilemelerini dağıtımdan önce yakalayın. Açık Kaynak projeleri için sonsuza kadar ücretsiz.
  * [coveralls.io](https://coveralls.io/) - Test kapsamı raporlarını görüntüleyin, Açık Kaynak için ücretsiz
  * [deepscan.io](https://deepscan.io) - JavaScript kodundaki çalışma zamanı hatalarını otomatik olarak bulmak için gelişmiş statik analiz, Açık Kaynak için ücretsiz
  * [DeepSource](https://deepsource.io/) - DeepSource kaynak kodu değişikliklerini sürekli olarak analiz eder; güvenlik, performans, anti-kalıplar, hata riskleri, dokümantasyon ve stil altında kategorize edilen sorunları bulur ve düzeltir. GitHub, GitLab ve Bitbucket ile yerel entegrasyon.
  * [DiffText](https://difftext.com) - İki kod bloğu arasındaki farkları anında bulun. Kullanımı tamamen ücretsizdir.
  * [eversql.com](https://www.eversql.com/) - EverSQL - Veritabanı optimizasyonu için 1 numaralı platform. Veritabanınıza ve SQL sorgularınıza ilişkin kritik öngörüleri otomatik olarak elde edin.
  * [gerrithub.io](https://review.gerrithub.io/) - GitHub depoları için ücretsiz Gerrit kodu incelemesi
  * [goreportcard.com](https://goreportcard.com/) - Go projeleri için Kod Kalitesi, Açık Kaynak için ücretsiz
  * [gtmetrix.com](https://gtmetrix.com/) - Web sitelerini optimize etmeye yönelik raporlar ve kapsamlı öneriler
  * [holistic.dev](https://holistic.dev/) - Postgresql optimizasyonu için 1 numaralı statik kod analizörü. Performans, güvenlik ve mimari veritabanı sorunlarının otomatik tespit hizmeti
  * [houndci.com](https://houndci.com/) - GitHub'un kod kalitesiyle ilgili taahhütleri hakkında yorumlar, Açık Kaynak için ücretsiz
  * [reviewable.io](https://reviewable.io/) - GitHub depoları için kod incelemesi, genel veya kişisel depolar için ücretsiz.
  * [scan.coverity.com](https://scan.coverity.com/) - Java, C/C++, C# ve JavaScript için statik kod analizi, Açık Kaynak için ücretsiz
  * [scrutinizer-ci.com](https://scrutinizer-ci.com/) - Sürekli inceleme platformu, Açık Kaynak için ücretsiz
  * [semanticdiff.com](https://app.semanticdiff.com/) - GitHub çekme istekleri ve taahhütleri için programlama diline duyarlı fark, genel depolar için ücretsiz
  * [shields.io](https://shields.io) - Açık kaynaklı projeler için kaliteli meta veri rozetleri
  * [sonarcloud.io](https://sonarcloud.io) - Java, JavaScript, C/C++, C#, VB.NET, PHP, Objective-C, Swift, Python, Groovy ve daha fazla dil için otomatik kaynak kodu analizi, Açık Kaynak için ücretsiz

**[⬆️Başa Dön](#table-of-contents)**

## Code Search and Browsing

  * [CodeKeep](https://codekeep.io) - Kod Parçacıkları için Google Keep. Ön ayarlı şablonlara ve bağlantı özelliğine sahip güçlü bir kod ekran görüntüsü aracı içeren kod parçacıklarını düzenleyin, keşfedin ve paylaşın.
  * [libraries.io](https://libraries.io/) - 32 farklı paket yöneticisi için arama ve bağımlılık güncelleme bildirimleri, açık kaynak için ücretsiz
  * [Namae](https://namae.dev/) - Proje adınızın kullanılabilirliği için GitHub, Gitlab, Heroku, Netlify ve çok daha fazlası gibi çeşitli web sitelerinde arama yapın.
  * [tickgit.com](https://www.tickgit.com/) - İyileştirme için geri dönmeye değer kod alanlarını belirlemek için "TODO" yorumlarını (ve diğer işaretçileri) ortaya çıkarır.

**[⬆️Başa Dön](#table-of-contents)**

## CI and CD

  * [appcircle.io](https://appcircle.io) - Daha hızlı, verimli sürüm döngüsü için mobil uygulamaların oluşturulmasını, test edilmesini ve yayınlanmasını otomatikleştiren kurumsal düzeyde bir mobil DevOps platformu. Derleme başına maksimum 30 dakikalık derleme süresi, 20 aylık derleme ve 1 eşzamanlı derleme için ücretsiz.
  * [appveyor.com](https://www.appveyor.com/) - Windows için CD hizmeti, Açık Kaynak için ücretsiz
  * [bitrise.io](https://www.bitrise.io/) - Yerel veya karma mobil uygulamalar için bir CI/CD. Ayda 200 ücretsiz derleme, 10 dakikalık derleme süresi ve iki ekip üyesiyle. OSS projeleri 45 dakikalık derleme süresi, +1 eşzamanlılık ve sınırsız ekip boyutu elde eder.
  * [buddy.works](https://buddy.works/) - Beş ücretsiz proje ve bir eşzamanlı çalıştırma (ayda 120 yürütme) içeren bir CI/CD
  * [Buildkite](https://buildkite.com) - CI Pipelines 3 kullanıcı için ücretsiz ve ayda 5 bin iş dakikası. Analitikleri ücretsiz test edin
geliştirici katmanı, açık kaynaklı projeler için daha fazla ücretsiz katılımla birlikte ayda 100.000 test yürütmesi içerir.
  * [bytebase.com](https://www.bytebase.com/) - Veritabanı CI/CD ve DevOps. 20'den az kullanıcı ve on veritabanı örneği ücretsiz
  * [CircleCI](https://circleci.com/) - GitHub, GitLab ve BitBucket depoları için barındırılan bir CI/CD hizmetinde bulunan tüm özellikleri içeren kapsamlı ücretsiz plan. Çoklu kaynak sınıfları, Docker, Windows, Mac OS, ARM yürütücüleri, yerel çalıştırıcılar, test bölme, Docker Katmanı Önbelleğe Alma ve diğer gelişmiş CI/CD özellikleri. Ayda 6000 dakikaya kadar yürütme süresi, sınırsız ortak çalışan, özel projelerde 30 paralel iş ve Açık Kaynak projeleri için 80.000'e kadar ücretsiz derleme dakikası için ücretsiz.
  * [cirrus-ci.org](https://cirrus-ci.org) - Herkese açık GitHub depoları için ücretsiz
  * [cirun.io](https://cirun.io) - Herkese açık GitHub depoları için ücretsiz
  * [codemagic.io](https://codemagic.io/) - Ayda 500 derleme dakikası ücretsiz
  * [deployhq.com](https://www.deployhq.com/) - Günlük on dağıtım içeren 1 proje (ayda 30 derleme dakikası)
  * [LocalOps](https://localops.co/) - Uygulamanızı 30 dakikadan kısa sürede AWS/GCP/Azure'da dağıtın. Yerleşik sürekli dağıtım otomasyonu ve gelişmiş gözlemlenebilirlik özellikleriyle birlikte herhangi bir bulutta standartlaştırılmış uygulama ortamları kurun. Ücretsiz plan 1 kullanıcıya ve 1 uygulama ortamına izin verir.
  * [Make](https://www.make.com/en) - İş akışı otomasyon aracı, kullanıcı arayüzünü kullanarak uygulamaları bağlamanıza ve iş akışlarını otomatikleştirmenize olanak tanır. Birçok uygulamayı ve en popüler API'leri destekler. Herkese açık GitHub depoları için ücretsiz ve 100 Mb, 1000 İşlem ve 15 dakikalık minimum aralıkla ücretsiz katman.
  * [Mergify](https://mergify.com) - GitHub için iş akışı otomasyonu ve birleştirme kuyruğu - Genel GitHub depoları için ücretsiz
  * [Nx Cloud](https://nx.dev/ci) - Nx Cloud, uzaktan önbelleğe alma, görevlerin makineler arasında dağıtılması ve hatta e2e test çalıştırmalarınızın otomatik olarak bölünmesi gibi özelliklerle CI'daki monorepo'larınızı hızlandırır. 150.000 cömert kredi içeren 30'a kadar katılımcı için ücretsiz bir planla birlikte gelir.
  * [RunMyJob](https://runmyjob.io) - Spike Örneklerini gerçek zamanlı ölçeklendirmeyle GitHub Actions ve GitLab CI işlem hatlarını daha akıllı çalıştırın. Ücretsiz katman, 400 vCPU-dakika, 800 GB-dakika ve yüksek performanslı çalıştırıcılarla (iş başına 12 vCPU ve 32 GB RAM) 10 eşzamanlı işi içerir.
  * [Shipfox](https://www.shipfox.io/) - GitHub eylemlerinizi 2 kat daha hızlı, her ay 3.000 derleme dakikası ücretsiz çalıştırın.
  * [Spacelift](https://spacelift.io/) - Kod Olarak Altyapı için yönetim platformu. Ücretsiz plan özellikleri: IaC işbirliği, Terraform modül kaydı, ChatOps entegrasyonu, Açık Politika Aracısı ile sürekli kaynak uyumu, SAML 2.0 ile SSO ve kamu çalışanı havuzlarına erişim: ayda 200 dakikaya kadar
  * [Squash Labs](https://www.squash.io/) - her şube için bir VM oluşturur ve uygulamanızı benzersiz bir URL'den, Sınırsız genel ve özel depolardan, 2 GB'a kadar VM Boyutlarından kullanılabilir hale getirir.
  * [Terramate](https://terramate.io/) - Terramate; Terraform, OpenTofu ve Terragrunt gibi Kod Olarak Altyapı (IaC) araçlarına yönelik bir düzenleme ve yönetim platformudur. Tüm özellikler dahil olmak üzere 2 kullanıcıya kadar ücretsiz.
  * [Terrateam](https://terrateam.io) - Çekme isteğine dayalı iş akışları, kendi kendine barındırılan çalıştırıcılar aracılığıyla proje izolasyonu ve sıralı işlemler için katmanlı çalıştırmalarla GitOps'un ilk Terraform otomasyonu. 3 kullanıcıya kadar ücretsizdir.

**[⬆️Başa Dön](#table-of-contents)**

## Testing

  * [Appetize](https://appetize.io) - Android ve iOS uygulamalarınızı bu Bulut Tabanlı Android Telefon / Tablet emülatöründe ve iPhone/iPad simülatörlerinde doğrudan tarayıcınızda test edin. Ücretsiz katman, ayda 30 dakikalık kullanımla eş zamanlı iki oturum içerir. Uygulama boyutunda sınırlama yoktur.
  * [Argos](https://argos-ci.com) - Geliştiriciler için Açık Kaynak görsel testi. Ayda 5.000 ekran görüntüsüyle sınırsız proje. Açık kaynaklı projeler için ücretsizdir.
  * [Bencher](https://bencher.dev/) - CI performans gerilemelerini yakalamak için sürekli bir kıyaslama araç paketi. Tüm kamu projeleri için ücretsizdir.
  * [BugBug](https://bugbug.io/) - Web uygulamaları için hafif test otomasyon aracı. Öğrenmesi kolaydır ve kodlama gerektirmez. Ücretsiz olarak kendi bilgisayarınızda sınırsız test çalıştırabilirsiniz. Ayrıca aylık ek ücret karşılığında bulut izleme ve CI/CD entegrasyonuna da sahip olursunuz.
  * [checkbot.io](https://www.checkbot.io/) - Web sitenizin 50'den fazla SEO, hız ve güvenlik en iyi uygulamalarına uyup uymadığını test eden tarayıcı uzantısı. Daha küçük web siteleri için ücretsiz katman.
  * [Checkly](https://checklyhq.com) - Modern DevOps için kod öncelikli sentetik izleme. API'lerinizi ve uygulamalarınızı eski sağlayıcıların fiyatının çok altında bir fiyata izleyin. Kod Olarak İzleme iş akışı ve Oyun Yazarı tarafından desteklenmektedir. Geliştiriciler için cömert ücretsiz katman.
  * [CORS-Tester](https://cors-error.dev/cors-tester/) - Geliştiricilerin ve API test uzmanlarının belirli bir alan için bir API'nin CORS uyumlu olup olmadığını kontrol etmelerine ve boşlukları belirlemelerine yönelik ücretsiz bir araç. Uygulanabilir bilgiler edinin.
  * [cypress.io](https://www.cypress.io/) - Tarayıcıda çalışan her şey için hızlı, kolay ve güvenilir test. Cypress Test Runner hiçbir kısıtlama ve sınırlama olmaksızın her zaman ücretsiz ve açık kaynaklıdır. Cypress Dashboard, 5 kullanıcıya kadar açık kaynaklı projeler için ücretsizdir.
  * [everystep-automation.com](https://www.everystep-automation.com/) - Bir web tarayıcısında gerçekleştirilen tüm adımları kaydeder ve tekrar oynatır ve daha az seçenekle ücretsiz olarak komut dosyaları oluşturur
  * [gridlastic.com](https://www.gridlastic.com/) - 4 adede kadar eşzamanlı Selenyum düğümü/10 ızgara başlangıcı/ayda 4.000 test dakikası içeren ücretsiz planla Selenyum Izgara testi
  * [katalon.com](https://katalon.com) - Katalon Studio, TestOps (+ Görsel Test ücretsiz), TestCloud ve Katalon Recorder dahil olmak üzere farklı test olgunluk düzeylerinde her büyüklükteki ekiplere yardımcı olabilecek bir test platformu sağlar.
  * [Keploy](https://keploy.io/) - Keploy, geliştiricilere yönelik işlevsel bir test araç setidir. API çağrılarının kaydedilmesi, API'ler (KTest'ler) ve modeller veya taslaklar (KMock'lar) için E2E testleri oluşturur. Açık Kaynak projeleri için ücretsizdir.
  * [loadmill.com](https://www.loadmill.com/) - Ağ trafiğini analiz ederek otomatik olarak API oluşturun ve testleri yükleyin. Aylık ücretsiz olarak 60 dakikaya kadar 50'ye kadar eşzamanlı kullanıcıyı simüle edin.
  * [lost-pixel.com](https://lost-pixel.com) - Hikaye Kitabınız, Pota, Tarih hikayeleriniz ve Web Uygulamalarınız için bütünsel görsel regresyon testi. Sınırsız ekip üyesi, açık kaynak için tamamen ücretsiz, ayda 7.000 anlık görüntü.
  * [pagegym.com](https://pagegym.com) - Davranış ve sayfa hızı analizi ve optimizasyon aracını yükleyin. Ücretsiz plan, günde 10 test, haftada 5 deney ve ayda maksimum 15 GB alınan veri sağlar.
  * [percy.io](https://percy.io) - Herhangi bir web uygulamasına, statik siteye, stil kılavuzuna veya bileşen kitaplığına görsel testler ekleyin.  Sınırsız ekip üyesi, Demo uygulaması ve sınırsız proje, ayda 5.000 anlık görüntü.
  * [qase.io](https://qase.io) - Geliştirme ve QA ekipleri için test yönetim sistemi. Test senaryolarını yönetin, test çalıştırmaları oluşturun, testler gerçekleştirin, kusurları takip edin ve etkiyi ölçün. Ücretsiz katman, ekler ve 3 kullanıcıya kadar kullanılabilen 500 MB ile tüm temel özellikleri içerir.
  * [Repeato](https://repeato.app/) - Bilgisayarla görme ve yapay zeka üzerine inşa edilmiş kodsuz mobil uygulama testi otomasyon aracı.
Yerel uygulamalar, flutter, react-native, web, ionic ve daha birçok uygulama çerçevesi için çalışır. Ücretsiz plan, iOS için 10 ve Android için 10 testle sınırlıdır, ancak sınırsız test çalıştırmaları da dahil olmak üzere ücretli planların çoğu özelliğini içerir.
  * [Requestly](https://requestly.com/) - HTTP İsteklerini Durdurmak, Yönlendirmek ve Sahte Etmek için Açık Kaynak Chrome Uzantısı.
[Hata Ayıklayıcı](https://requestly.com/products/web-debugger/), [Sahte Sunucu](https://requestly.com/products/mock-server/), [API İstemcisi](https://requestly.com/products/api-client/) ve [Oturum Kaydı](https://requestly.com/products/session-book/) özelliklerine sahiptir.  URL'leri yeniden yönlendirin, HTTP Başlıklarını Değiştirin, Sahte API'ler, Özel JS enjekte edin, GraphQL İsteklerini Değiştirin, Sahte API Uç Noktaları Oluşturun, Ağ ve Konsol Günlükleriyle oturumu kaydedin. Ücretsiz Katmanda en fazla 10 kural oluşturun. Açık kaynak için ücretsiz.
  * [seotest.me](https://seotest.me/) - Ücretsiz sayfa içi SEO web sitesi test aracı. Günde 10 ücretsiz web sitesi taraması. Teknolojiden bağımsız olarak herhangi bir web sitesi için sayfa içi SEO sonuçlarının nasıl iyileştirilebileceğine dair faydalı SEO öğrenme kaynakları ve öneriler.
  * [snippets.uilicious.com](https://snippets.uilicious.com) - CodePen'e benziyor ancak tarayıcılar arası test için. UI-licious, kullanıcı hikayeleri gibi testler yazmanıza olanak tanır ve ücretsiz bir platform (UI-licious Snippet'ler) sunar; bu, test çalıştırması başına 3 dakikaya kadar herhangi bir kayıt gerektirmeden Chrome'da sınırsız testler çalıştırmanıza olanak tanır. Bir hata mı buldunuz? Geliştiricilerinize hatayı tam olarak nasıl yeniden oluşturacaklarını göstermek için benzersiz URL'yi testinize kopyalayabilirsiniz.
  * [SSR (Sunucu Tarafı Oluşturma) Denetleyicisi](https://www.crawlably.com/ssr-checker/) - Sayfanın sunucu tarafından oluşturulan sürümünü normal sürümle görsel olarak karşılaştırarak herhangi bir URL için SSR'yi (sunucu tarafı oluşturma) kontrol edin.
  * [testingbot.com](https://testingbot.com/) - Selenyum Tarayıcı ve Cihaz Testi, [Açık Kaynak için ücretsiz](https://testingbot.com/open-source)
  * [Testspace.com](https://testspace.com/) - Otomatik test sonuçlarını yayınlamak için bir Kontrol Paneli ve GitHub kullanarak manuel testleri kod olarak uygulamak için bir Çerçeve. Hizmet [Açık Kaynak için ücretsizdir](https://github.com/marketplace/testspace-com) ve 450 aylık sonuç sağlar.
  * [tesults.com](https://www.tesults.com) - Test sonuçlarının raporlanması ve test senaryosu yönetimi. Popüler test çerçeveleriyle bütünleşir. Açık Kaynak yazılım geliştiricileri, bireyler, eğitimciler ve başlangıç ​​aşamasındaki küçük ekipler, temel ücretsiz projelerin ötesinde indirimli ve ücretsiz teklifler talep edebilir.
  * [UseWebhook.com](https://usewebhook.com) - Tarayıcınızdan web kancalarını yakalayın ve inceleyin. Localhost'a iletin veya geçmişten tekrar oynatın. Kullanımı ücretsiz.
  * [Vaadin](https://vaadin.com) - Java veya TypeScript'te ölçeklenebilir kullanıcı arayüzleri oluşturun ve daha hızlı yineleme yapmak, daha iyi tasarım yapmak ve geliştirme sürecini basitleştirmek için entegre araçları, bileşenleri ve tasarım sistemini kullanın. Beş yıllık ücretsiz bakımla Sınırsız Proje.
  * [webhook-test.com](https://webhook-test.com) - Entegrasyon sırasında benzersiz bir URL ile web kancalarında ve HTTP isteklerinde hata ayıklayın ve inceleyin. Tamamen ücretsiz olup sınırsız URL oluşturabilir ve öneriler alabilirsiniz.
  * [webhook.site](https://webhook.site) - Özel bir URL ile web kancalarını, giden HTTP isteklerini veya e-postaları doğrulayın. Geçici bir URL ve e-posta adresi her zaman ücretsizdir.
  * [websitepulse.com](https://www.websitepulse.com/tools/) - Çeşitli ücretsiz ağ ve sunucu araçları.
  * [kogiQA](https://kogiqa.com) - Seçicilere ihtiyaç duymadan çalışan bir web kullanıcı arayüzü otomasyon aracı. Her geliştirici ayda 500 işlemden ücretsiz olarak yararlanır.

**[⬆️Başa Dön](#table-of-contents)**

## Security and PKI

  * [aikido.dev](https://www.aikido.dev) - SCA, SAST, CSPM, DAST, Secrets, IaC, Malware, Container tarama, EOL,...'yi kapsayan hepsi bir arada uygulama platformu. Ücretsiz planda iki kullanıcı, 10 depo, 1 bulut, 2 konteyner ve 1 alan taraması bulunur.
  * [CertKit](https://www.certkit.io/certificate-management) - SSL Sertifikası verilmesini, yenilenmesini ve izlenmesini yönetin. Sertifika Şeffaflığı Günlüklerinde arama yapın. Betadan sonra 3 sertifika ve 1 kullanıcı için ücretsiz.
  * [Corgea](https://corgea.com/) - +20 dil ve çerçeve genelinde güvenli olmayan kod ve paketleri bulan, doğrulayan ve düzelten ücretsiz otonom güvenlik platformu. Ücretsiz plan 1 kullanıcı ve 2 depo içerir.
  * [crypteron.com](https://www.crypteron.com/) - Bulut öncelikli, geliştirici dostu güvenlik platformu, .NET ve Java uygulamalarındaki veri ihlallerini önler
  * [CyberChef](https://gchq.github.io/CyberChef/) - Karmaşık araçlarla veya programlama dilleriyle uğraşmadan verileri analiz etmek ve kodunu çözmek/kodlamak için basit, sezgisel bir web uygulaması. Kriptografi ve şifrelemede İsviçre çakısı gibi. Tüm özelliklerin kullanımı ücretsizdir ve herhangi bir sınırlama yoktur. Kendi kendine barındırmak istiyorsanız açık kaynak.
  * [Datree](https://www.datree.io/) - Manifestlerin ve Helm grafiklerinin kuruluşunuzun politikalarının yanı sıra en iyi uygulamaları takip etmesini sağlayarak Kubernetes'te yanlış yapılandırmaları önleyen Açık Kaynak CLI aracı
  * [Dependabot](https://dependabot.com/) - Ruby, JavaScript, Python, PHP, Elixir için otomatik bağımlılık güncellemeleri,
Rust, Java (Maven ve Gradle), .NET, Go, Elm, Docker, Terraform, Git Alt Modülleri ve GitHub Eylemleri.
  * [DJ Checkup](https://djcheckup.com) - Bu ücretsiz, otomatik kontrol aracıyla Django sitenizi güvenlik açıklarına karşı tarayın. Pony Checkup sitesinden çatallanmıştır.
  * [Doppler](https://doppler.com/) - Çeşitli bulut sağlayıcılarıyla senkronizasyon desteğiyle uygulama sırları ve yapılandırması için Evrensel Sırlar Yöneticisi. Temel erişim kontrollerine sahip beş kullanıcı için ücretsizdir.
  * [Dotenv](https://dotenv.org/) - .env dosyalarınızı hızlı ve güvenli bir şekilde senkronize edin. .env dosyalarınızı Slack ve e-posta gibi güvenli olmayan kanallar üzerinden paylaşmayı bırakın ve önemli bir .env dosyasını bir daha asla kaybetmeyin. En fazla 3 takım arkadaşına ücretsiz.
  * [GitGuardian](https://www.gitguardian.com) - Otomatik gizli dizi algılama ve düzeltme özelliğiyle sırları kaynak kodunuzdan uzak tutun. Git depolarınızı 350'den fazla türde sır ve hassas dosya için tarayın - Bireyler ve 25 veya daha az geliştiriciden oluşan ekipler için ücretsiz.
  * [HasMySecretLeaked](https://gitguardian.com/hasmysecretleaked) - Herkese açık GitHub depolarında, özetlerde, sorunlarda ve yorumlarda açığa çıkan 20 milyon gizli bilgiyi Ücretsiz olarak arayın
  * [Pwned oldum mu?](https://haveibeenpwned.com) - İhlallerle ilgili bilgileri almak için REST API.
  * [hostedscan.com](https://hostedscan.com) - Web uygulamaları, sunucular ve ağlar için çevrimiçi güvenlik açığı tarayıcısı. Ayda on ücretsiz tarama.
  * [Infisical](https://infisical.com/) - Ekibiniz ve altyapınız genelinde geliştirici sırlarını yönetmenize olanak tanıyan açık kaynak platform: yerel geliştirmeden hazırlama/üretim 3. taraf hizmetlerine kadar her yerde. 5 geliştiriciye kadar ücretsiz.
  * [Internet.nl](https://internet.nl) - IPv6, DNSSEC, HTTPS, DMARC, STARTTLS ve DANE gibi modern İnternet Standartlarını test edin
  * [IntoDNS.ai](https://intodns.ai) - SPF, DKIM, DMARC, DNSSEC, BIMI, MTA-STS ve 40'tan fazla kara listeyi yapay zeka destekli açıklamalar ve düzeltme önerileriyle kontrol eden DNS ve e-posta güvenlik analizörü. %100 ücretsiz, kayıt olmanıza gerek yok.
  * [letsencrypt.org](https://letsencrypt.org/) - Tüm büyük tarayıcıların güvendiği sertifikalara sahip Ücretsiz SSL Sertifika Yetkilisi
  * [meterian.io](https://www.meterian.io/) - Java, Javascript, .NET, Scala, Ruby ve NodeJS projelerini bağımlılıklardaki güvenlik açıklarına karşı izleyin. Bir özel proje için ücretsiz, açık kaynak için sınırsız proje.
  * [Mozilla Gözlemevi](https://observatory.mozilla.org/) - Sitenizdeki güvenlik açıklarını bulun ve düzeltin.
  * [Project Gatekeeper](https://gatekeeper.binarybiology.top/) - Özel Anahtar ve CSR Oluşturucu, SSL Sertifika Kod Çözücü, Sertifika Eşleştirici ve Sipariş SSL Sertifikası gibi çeşitli özellikler sunan Hepsi Bir Arada SSL Araç Seti. Kullanıcılarımıza TXT Kayıtları yerine CNAME Kayıtlarını kullanarak Let's Encrypt, Google Trust ve BuyPass'tan Ücretsiz SSL Sertifikaları oluşturmalarını sunuyoruz.
  * [Protectumus](https://protectumus.com) - PHP için ücretsiz web sitesi güvenlik kontrolü, site antivirüsü ve sunucu güvenlik duvarı (WAF). Ücretsiz katmandaki kayıtlı kullanıcılar için e-posta bildirimleri.
  * [Genel Bulut Tehdit İstihbaratı](https://cloudintel.himanshuanand.com/) - Genel bulut altyapısını hedefleyen yüksek güvenliğe sahip Tehlike Göstergesi (IOC), Bir kısmı github'da mevcut (https://github.com/unknownhad/AWSAttacks). Tam liste API aracılığıyla mevcut)
  * [pyup.io](https://pyup.io) - Python bağımlılıklarını güvenlik açıklarına karşı izleyin ve bunları otomatik olarak güncelleyin. Bir özel proje için ücretsiz, açık kaynak için sınırsız proje.
  * [qualys.com](https://www.qualys.com/community-edition) - Web uygulaması güvenlik açıklarını bulun, OWASP Risklerini denetleyin
  * [Smart Grow Vault](https://vault.smart-grow.app/) - Ortam değişkenlerini ve sırlarını yönetmek için Güvenli Kurumsal düzeyde platform. Ücretsiz katman, proje başına en fazla 3 uygulama ve 150 gizli dizi içerir.
  * [Socket](https://socket.dev) - Bireysel geliştiriciler, küçük ekipler ve açık kaynak projeleri için ücretsiz tedarik zinciri güvenliği. Kodunuzu savunmasız ve kötü niyetli bağımlılıklardan korumak için ücretsiz bir uygulama ve güvenlik duvarı CLI aracı içerir. Tedarik zinciri riskine ilişkin 70'ten fazla göstergeyi tespit eder.
  * [SOOS](https://soos.io) - Açık kaynaklı projeler için ücretsiz, sınırsız SCA taraması. Güvenlik tehditlerini yayınlanmadan önce tespit edin ve düzeltin. Basit ve etkili bir çözümle projelerinizi koruyun.
  * [ssllabs.com](https://www.ssllabs.com/ssltest/) - Herhangi bir SSL web sunucusunun yapılandırmasının yoğun analizi
  * [Sucuri SiteCheck](https://sitecheck.sucuri.net) - Ücretsiz web sitesi güvenlik kontrolü ve kötü amaçlı yazılım tarayıcısı
  * [TestTLS.com](https://testtls.com) - Güvenli sunucu yapılandırması, sertifikalar, zincirler vb. için bir SSL/TLS hizmetini test edin. HTTPS ile sınırlı değildir.
  * [Virgil Security](https://virgilsecurity.com/) - Dijital çözümünüzde uçtan uca şifreleme, veritabanı koruması, IoT güvenliği ve daha fazlasını uygulamaya yönelik araçlar ve hizmetler. 250 kullanıcıya kadar olan uygulamalar için ücretsizdir.

**[⬆️Başa Dön](#table-of-contents)**

## Authentication, Authorization, and User Management

  * [360username](https://360username.com/) - Eşleşen profilleri bulmak için 90'dan fazla sosyal platformda bir kullanıcı adını aramak için ücretsiz bir araç.
  * [Aserto](https://www.aserto.com) - Uygulamalar ve API'ler için bir hizmet olarak ayrıntılı yetkilendirme. 1000'e kadar MAU'ya ve 100 yetkilendirme örneğine kadar ücretsiz.
  * [asgardeo.io](https://wso2.com/asgardeo) - SSO, MFA, şifresiz kimlik doğrulama ve daha fazlasının Sorunsuz Entegrasyonu. Ön uç ve arka uç uygulamaları için SDK'lar içerir. 1000'e kadar MAU ve beş kimlik sağlayıcıya kadar ücretsiz.
  * [Auth0](https://auth0.com/) - Barındırılan SSO. Ücretsiz plan 25.000 MAU, sınırsız Sosyal Bağlantı, özel bir alan adı ve daha fazlasını içerir.
  * [Authgear](https://www.authgear.com) - Uygulamalarınıza birkaç dakika içinde Şifresiz, OTP'ler, 2FA ve SSO'yu getirin. Tüm Ön Uç dahildir. 5000 MAU'ya kadar ücretsiz.
  * [Authress](https://authress.io/) - Kimlik doğrulama oturum açma ve erişim kontrolü, herhangi bir proje için sınırsız kimlik sağlayıcıları. Facebook, Google, Twitter ve daha fazlası. İlk 1000 API çağrısı ücretsizdir.
  * [Authy](https://authy.com) - Yedeklemelerle birden fazla cihazda iki faktörlü kimlik doğrulama (2FA). Google Authenticator için açılır değiştirme. 100'e kadar başarılı kimlik doğrulama için ücretsiz.
  * [Cerbos Hub](https://www.cerbos.dev/product-cerbos-hub) - Erişim politikalarını yazmak, test etmek ve dağıtmak için eksiksiz bir yetkilendirme yönetim sistemi. Ayrıntılı yetkilendirme ve erişim kontrolü, 100 aya kadar aktif sorumluya kadar ücretsiz.
  * [Katip](https://clerk.com) - Kullanıcı yönetimi, kimlik doğrulama, 2FA/MFA, oturum açma, kaydolma, kullanıcı profilleri ve daha fazlası için önceden oluşturulmuş kullanıcı arayüzü bileşenleri. Ücretsiz planda sınırsız uygulama, uygulama başına 50.000 MRU sınırı, 3 kontrol paneli koltuğu ve daha fazlası bulunur.
  * [Cloud-IAM](https://www.cloud-iam.com/) - Bir Hizmet Olarak Keycloak Kimlik ve Erişim Yönetimi. 100 kullanıcıya ve bir bölgeye kadar ücretsiz.
  * [Descope](https://www.descope.com/) - Yüksek düzeyde özelleştirilebilir Kimlik Doğrulama akışları, hem kodsuz hem de API/SDK yaklaşımına sahiptir, Ücretsiz 7.500 aktif kullanıcı/ay, 50 kiracı (en fazla 5 SAML/SSO kiracısı).
  * [duo.com](https://duo.com/) - Web sitesi veya uygulama için iki faktörlü kimlik doğrulama (2FA). On kullanıcı için ücretsiz, tüm kimlik doğrulama yöntemleri, sınırsız, entegrasyonlar, donanım belirteçleri.
  * [Kinde](https://kinde.com/) - Birkaç dakika içinde ürününüze entegre edebileceğiniz basit, sağlam kimlik doğrulama.  7.500 ücretsiz MAU ile başlamak için ihtiyacınız olan her şey.
  * [logintc.com](https://www.logintc.com/) - Anlık bildirimlerle iki faktörlü kimlik doğrulama (2FA), on kullanıcı için ücretsiz, VPN, Web siteleri ve SSH
  * [Logto](https://logto.io/) - Hem kimlik doğrulama hem de yetkilendirme için ürününüzün kullanıcı kimliklerini geliştirin, güvenliğini sağlayın ve yönetin. Açık kaynaklı, kendi kendine barındırılan seçeneğiyle 5.000 MAU'ya kadar ücretsiz.
  * [MojoAuth](https://mojoauth.com/) - MojoAuth, Parolasız kimlik doğrulamayı web'inizde, mobil cihazınızda veya herhangi bir uygulamada dakikalar içinde uygulamayı kolaylaştırır.
  * [Okta](https://developer.okta.com/signup/) - Kullanıcı yönetimi, kimlik doğrulama ve yetkilendirme. Aylık 100 aktif kullanıcıya kadar ücretsizdir.
  * [Ory](https://ory.sh/) - AuthN/AuthZ/OAuth2.0/Zero Trust yönetilen güvenlik platformu. Tüm güvenlik özelliklerine, sınırsız ekip üyesine, 200 günlük aktif kullanıcıya ve ayda 25 bin izin kontrolüne sahip sonsuza kadar ücretsiz geliştirici hesapları.
  * [Permit.io](https://permit.io) - Gerçek zamanlı güncellemeler ve kodsuz politika kullanıcı arayüzü ile ölçeklenebilir mikro hizmetler için RBAC, ABAC ve ReBAC'ı etkinleştiren hizmet olarak kimlik doğrulama sağlayıcı platformu. 1000 Aylık Aktif Kullanıcı ücretsiz kullanımı.
  * [İkinci Aşama](https://phasetwo.io) - Keycloak Açık Kaynak Kimliği ve Erişim Yönetimi. 1000 kullanıcıya kadar ücretsiz bölge, 10'a kadar SSO bağlantısı, İkinci Aşamanın [Organizasyon](https://phasetwo.io/product/organizations/) uzantısını içeren Keycloak geliştirilmiş kapsayıcısından yararlanıyor.
  * [PropelAuth](https://propelauth.com) - Birkaç satır kodla, 200 kullanıcıya kadar ücretsiz ve 10.000 İşlemsel E-postayla (filigran markasıyla: "Powered by PropelAuth") her büyüklükteki şirkete anında satış yapın.
  * [Scalekit](https://scalekit.com) - Kurumsal SSO (SAML, OIDC), SCIM sağlama ve B2B SaaS için sosyal oturum açma işlemleri. Ücretsiz katman 1 milyon MAU, 100 kuruluş, 1 SSO bağlantısı ve 1 SCIM bağlantısını içerir.
  * [Stack Auth](https://stack-auth.com) - Berbat olmayan açık kaynak kimlik doğrulaması. Yalnızca beş dakika içinde başlamanızı sağlayan en geliştirici dostu çözüm. Ücretsiz olarak kendi kendine barındırılabilir veya 10.000 ücretsiz Aylık Aktif Kullanıcıya sahip yönetilen bir SaaS sürümü sunar.
  * [Stytch](https://www.stytch.com/) - Kimlik doğrulama ve sahtekarlığın önlenmesi için API'ler ve SDK'lar sağlayan hepsi bir arada platform. Ücretsiz plan, 10.000 aylık aktif kullanıcı, sınırsız organizasyon, 5 SSO veya SCIM bağlantısı ve 1.000 M2M token içerir.
  * [SuperTokens](https://supertokens.com/) - Uygulamanıza yerel olarak entegre olan açık kaynaklı kullanıcı kimlik doğrulaması, kullanıcı ve geliştirici deneyimini kontrol ederken hızlı bir şekilde başlamanıza olanak tanır. 5000 MAU'ya kadar ücretsiz.
  * [WorkOS](https://workos.com/) - 1 Milyon MAU'ya kadar ücretsiz kullanıcı yönetimi ve kimlik doğrulama. E-posta + şifre, sosyal kimlik doğrulama, Magic Auth, MFA ve daha fazlasını destekleyin.
  * [ZITADEL Cloud](https://zitadel.com) - Sizin için çalışan ve çok kiracılı (B2B) kullanım örneklerini destekleyen anahtar teslimi bir kullanıcı ve erişim yönetimi. Tüm güvenlik özellikleriyle (OTP, Parolasız, Politikalar vb. için ödeme duvarı yok) 25.000'e kadar kimlik doğrulamalı istek için ücretsiz.


**[⬆️Başa Dön](#table-of-contents)**

## Mobile App Distribution and Feedback

  * [Appho.st](https://appho.st) - Mobil uygulama barındırma platformu. Ücretsiz planda beş uygulama, 50 aylık indirme ve maksimum 100 MB dosya boyutu bulunur.
  * [Diawi](https://www.diawi.com) - iOS ve Android uygulamalarını doğrudan cihazlara dağıtın. Ücretsiz plan: uygulama yüklemeleri, şifre korumalı bağlantılar, 1 günlük son kullanma tarihi, on kurulum.
  * [GetUpdraft](https://www.getupdraft.com) - Mobil uygulamaları test için dağıtın. Ücretsiz plan, bir uygulama projesi, üç uygulama sürümü, 500 MB depolama alanı ve ayda 100 uygulama yüklemesini içerir.
  * [InstallOnAir](https://www.installonair.com) - iOS ve Android uygulamalarını kablosuz olarak dağıtın. Ücretsiz plan: sınırsız yükleme, özel bağlantılar, misafirler için 2 günlük süre sonu, kayıtlı kullanıcılar için 60 gün.
  * [Loadly](https://loadly.io) - iOS ve Android beta uygulama dağıtım hizmeti, sınırsız indirme, yüksek hızlı indirme ve sınırsız yükleme ile tamamen ücretsiz hizmetler sunar.

**[⬆️Başa Dön](#table-of-contents)**

## Management System

  * [bitnami.com](https://bitnami.com/) - Hazırlanan uygulamaları IaaS'de dağıtın. 1 AWS mikro örneğinin yönetimi ücretsiz
  * [Esper](https://esper.io) - DevOps özellikli Android Cihazlar için MDM ve MAM. Bir kullanıcı lisansı ve 25 MB Uygulama Depolama Alanı ile yüz cihaz ücretsiz.
  * [jamf.com](https://www.jamf.com/) - iPad'ler, iPhone'lar ve Mac'ler için cihaz yönetimi, üç cihaz ücretsiz
  * [Miradore](https://miradore.com) - Cihaz Yönetimi hizmeti. Cihaz filonuzla güncel kalın ve sınırsız cihazı ücretsiz olarak güvence altına alın. Ücretsiz plan temel özellikler sunar.
  * [moss.sh](https://moss.sh) - Geliştiricilerin web uygulamalarını ve sunucularını dağıtmalarına ve yönetmelerine yardımcı olun. Ayda 25 git dağıtımına kadar ücretsiz
  * [ploi.io](https://ploi.io/) - Sunucularınızı ve sitelerinizi kolayca yönetmek ve dağıtmak için sunucu yönetimi aracı. Bir sunucu için ücretsiz.
  * [runcloud.io](https://runcloud.io/) - Esas olarak PHP projelerine odaklanan sunucu yönetimi. 1 sunucuya kadar ücretsiz.
  * [serveravatar.com](https://serveravatar.com) - PHP tabanlı web sunucularını otomatik yapılandırmalarla yönetin ve izleyin. Bir sunucu için ücretsiz.
  * [xcloud.host](https://xcloud.host) - Kullanıcı dostu bir arayüze sahip sunucu yönetimi ve dağıtım platformu. Bir sunucu için ücretsiz katman mevcuttur.

**[⬆️Başa Dön](#table-of-contents)**

## Messaging and Streaming

  * [Ably](https://www.ably.com/) - Mevcudiyet, kalıcılık ve garantili teslimat ile gerçek zamanlı mesajlaşma hizmeti. Ücretsiz plan ayda 3 milyon mesaj, 100 yoğun bağlantı ve 100 yoğun kanal içerir.
  * [cloudamqp.com](https://www.cloudamqp.com/) - Hizmet olarak RabbitMQ. Küçük Lemur planı: ayda maksimum 1 milyon mesaj, maksimum 20 eşzamanlı bağlantı, maksimum 100 kuyruk, maksimum 10.000 sıraya alınmış mesaj, farklı AZ'lerde birden fazla düğüm
  * [courier.com](https://www.courier.com/) - Push, uygulama içi, e-posta, sohbet, SMS ve şablon yönetimi ve diğer özelliklere sahip diğer mesajlaşma kanalları için tek API. Ücretsiz plan ayda 10.000 mesaj içerir.
  * [EMQX Sunucusuz](https://www.emqx.com/en/cloud/serverless-mqtt) - Saniyeler içinde alabileceğiniz ölçeklenebilir ve güvenli sunucusuz MQTT komisyoncusu. 1 milyon oturum dakikası/ay sonsuza kadar ücretsiz (kredi kartı gerekmez).
  * [Engage](https://engage.so/) - SaaS için Hepsi Bir Arada Müşteri Etkileşimi ve Otomasyon Aracı (e-posta, push, SMS, ürün turları, afişler ve daha fazlası). Ayda 1.000 aktif kullanıcıya kadar ücretsizdir.
  * [engagespot.co](https://engagespot.co/) - Önceden oluşturulmuş uygulama içi gelen kutusu ve kodsuz şablon düzenleyiciye sahip, geliştiriciler için çok kanallı bildirim altyapısı. Ücretsiz plan ayda 10.000 mesaj içerir.
  * [HiveMQ](https://www.hivemq.com/mqtt-cloud-broker/) - MQTT cihazlarınızı Cloud Native IoT Messaging Broker'a bağlayın.  Sonsuza kadar 100 cihaza kadar ücretsiz bağlantı (kredi kartı gerekmez).
  * [httpSMS](https://httpsms.com) - Android telefonunuzu SMS Ağ Geçidi olarak kullanarak kısa mesaj gönderin ve alın. Ayda 200'e kadar mesaj göndermek ve almak ücretsizdir.
  * [knock.app](https://knock.app) - Geliştiriciler için bildirim altyapısı. Tek bir API çağrısıyla uygulama içi, e-posta, SMS, Slack ve push gibi birden fazla kanala gönderin. Ücretsiz plan ayda 10.000 mesaj içerir.
  * [Novu.co](https://novu.co) - Geliştiriciler için açık kaynaklı bildirim altyapısı. Tüm iletişim kanallarını tek bir yerden yönetmek için basit bileşenler ve API'ler: E-posta, SMS, Doğrudan, Uygulama İçi ve Push. Ücretsiz plan, 90 günlük saklama süresiyle ayda 30.000 bildirim içerir.
  * [Pingram.io](https://www.pingram.io/) - 5 dakikada iletişim altyapısı. Ücretsiz kullanım şunları içerir: 100 SMS ve arama, 3000 E-posta, Push, Slack, MS Teams, WhatsApp ve daha fazlası.
  * [Cep Uyarısı](https://pocketalert.app) - iOS ve Android cihazlarınıza anında bildirimler gönderin. API veya Web Kancaları aracılığıyla zahmetsizce entegre olun ve uyarılarınız üzerinde tam kontrol sağlayın. Ücretsiz plan: 1 cihaza ve 1 uygulamaya günde 50 mesaj.
  * [pubnub.com](https://www.pubnub.com/) - Swift, Kotlin ve React mesajlaşması her ay 1 milyon işlemde. İşlemler birden fazla mesaj içerebilir.
  * [pusher.com](https://pusher.com/) - Gerçek zamanlı mesajlaşma hizmeti. 100'e kadar eşzamanlı bağlantı ve günde 200.000 mesaja kadar ücretsiz
  * [scaledrone.com](https://www.scaledrone.com/) - Gerçek zamanlı mesajlaşma hizmeti. 20'ye kadar eşzamanlı bağlantı ve günde 100.000 etkinlik için ücretsiz
  * [SMSGate](https://sms-gate.app) - Android™ için SMS Ağ Geçidi, bulut yönlendirmeyi kullanarak cihazlarınız aracılığıyla SMS mesajları gönderip almanızı sağlar. Tamamen ücretsiz bulut hizmeti (tüm kullanıcılar için kaliteyi korumak amacıyla günde 10.000 mesajın üzerinde kullanım için önerilen bildirimle birlikte).
  * [SuprSend](https://www.suprsend.com/) - SuprSend, ürün bildirimlerinizi API öncelikli bir yaklaşımla kolaylaştıran bir bildirim altyapısıdır. Tek bir bildirim API'si ile birden fazla kanalda işlem, cron ve etkileşim bildirimleri oluşturun ve iletin. Ücretsiz planda özetler, gruplar, çoklu kanallar, tercihler, kiracılar, yayınlar ve daha fazlası gibi farklı iş akışı düğümleri dahil olmak üzere ayda 10.000 bildirim alırsınız.
  * [synadia.com](https://synadia.com/ngs) - [NATS.io](https://nats.io) bir hizmet olarak. Küresel, AWS, GCP ve Azure. 4k mesaj boyutu, 50 aktif bağlantı ve ayda 5 GB veriyle sonsuza kadar ücretsiz.
  * [webpushr](https://www.webpushr.com/) - Web Push Bildirimleri - 10.000'e kadar abone için ücretsiz, sınırsız push bildirimleri, tarayıcı içi mesajlaşma

**[⬆️Başa Dön](#table-of-contents)**

## Log Management

  * [bugfender.com](https://bugfender.com/) - 24 saat saklamayla günde 100.000'e kadar günlük satırı ücretsiz
  * [log.dog](https://log.dog/) - LogDog, web kullanıcı arayüzüne sahip uzaktan hata ayıklama/günlüğe kaydetme SDK'sıdır (iOS ve Android). Tüm günlükleri, istekleri ve olayları gerçek zamanlı olarak yakalar ve bunların ele geçirilmesine olanak tanır. Her ay 100 MB'a kadar günlük ücretsiz
  * [logflare.app](https://logflare.app/) - Uygulama başına ayda 12.960.000'e kadar ücretsiz giriş, 3 günlük saklama
  * [logtail.com](https://logtail.com/) - ClickHouse tabanlı SQL uyumlu günlük yönetimi. Ayda 1 GB'a kadar ücretsiz, üç günlük saklama.
  * [logzab.com](https://logzab.com/) - Denetim takibi yönetim sistemi. En fazla 5 proje için ayda 1.000 kullanıcı etkinliği günlüğü ücretsiz, 1 aylık saklama.
  * [ManageEngine Log360 Cloud](https://www.manageengine.com/cloud-siem/) - Manage Engine tarafından desteklenen Günlük Yönetimi hizmeti. Ücretsiz Plan, 15 günlük Depolama Saklama ve 7 günlük arama ile 50 GB depolama alanı sunar.
  * [openobserve.ai](https://openobserve.ai/) - 200 GB Kullanım/ay ücretsiz, 15 Gün Saklama
  * [Akıllı Büyüme Günlükleri](https://logs.smart-grow.app/) - Uçtan uca şifreleme, gerçek zamanlı uyarılar ve çok platformlu SDK'lara sahip merkezi günlük yönetimi platformu. Ücretsiz katman günde en fazla 3.000 günlük içerir.

**[⬆️Başa Dön](#table-of-contents)**

## Translation Management

  * [AutoLocalise.com](https://www.autolocalise.com/) - Çeviri dosyalarını yönetmeden anında yerelleştirin. Ayda 10.000 karaktere kadar ücretsiz, sınırsız dil.
  * [crowdin.com](https://crowdin.com/) - Açık Kaynak için sınırsız proje, sınırsız dize ve ortak çalışanlar
  * [Ücretsiz PO editörü](https://pofile.net/free-po-editor) - Herkes için ücretsiz
  * [Lingo.dev](https://lingo.dev) - Web ve mobil yerelleştirme için açık kaynaklı yapay zeka destekli CLI. Kendi LLM'nizi getirin veya Lingo.dev tarafından yönetilen yerelleştirme motoru aracılığıyla her ay 10.000 ücretsiz kelimeden yararlanın.
  * [lingohub.com](https://lingohub.com/) - 3 kullanıcıya kadar ücretsiz, Açık Kaynak için her zaman ücretsiz
  * [localazy.com](https://localazy.com) - 1000 kaynak dil dizesi, sınırsız dil, sınırsız katkıda bulunanlar, başlangıç ​​ve açık kaynak anlaşmaları için ücretsiz
  * [Localit](https://localit.io) - Sorunsuz ve ücretsiz GitHub/GitLab entegrasyonu, yapay zeka destekli ve manuel çeviriler ve cömert bir ücretsiz plan (2 kullanıcı, 500 anahtar ve sınırsız proje içerir) içeren hızlı, geliştirici dostu yerelleştirme platformu.
  * [localizely.com](https://localizely.com/) - Açık Kaynak için Ücretsiz
  * [Loco](https://localise.biz/) - 2000'e kadar ücretsiz çeviri, Sınırsız çevirmen, on dil/proje, 1000 çevrilebilir varlık/proje
  * [POEditor](https://poeditor.com/) - 1000 dizeye kadar ücretsiz
  * [SimpleLocalize](https://simplelocalize.io/) - 100'e kadar ücretsiz çeviri anahtarı, sınırsız dize, sınırsız dil, başlangıç ​​fırsatları
  * [Texterify](https://texterify.com/) - Tek bir kullanıcı için ücretsiz
  * [Tolgee](https://tolgee.io) - Sınırlı çevirilerle ücretsiz SaaS teklifi, sonsuza kadar ücretsiz, kendi kendine barındırılan sürüm
  * [transifex.com](https://www.transifex.com/) - Açık Kaynak için Ücretsiz

**[⬆️Başa Dön](#table-of-contents)**

## Monitoring

  * [assertible.com](https://assertible.com) - Otomatik API testi ve izleme. Ekipler ve bireyler için ücretsiz planlar.
  * [Better Stack](https://betterstack.com/better-uptime) - Tek bir üründe çalışma süresi izleme, olay yönetimi, çağrı üzerine planlama/uyarı ve durum sayfaları. Ücretsiz plan, 3 dakikalık kontrol sıklığı ve durum sayfalarına sahip on monitör içerir.
  * [bleemeo.com](https://bleemeo.com) - 3 sunucu, 5 çalışma süresi monitörü, sınırsız kullanıcı, sınırsız kontrol paneli, sınırsız uyarı kuralı için ücretsiz.
  * [checklyhq.com](https://checklyhq.com) - Geliştiriciler için açık kaynak E2E / Sentetik izleme ve derin API izleme. Tek kullanıcılı ve 10.000 API ve ağ / 1.5.000 tarayıcı kontrolü çalıştırmalı ücretsiz plan.
  * [Önemli Web Verileri Geçmişi](https://punits.dev/core-web-vitals-historical/) - Bir URL veya web sitesi için Önemli Web Verileri geçmişini bulun.
  * [cronitor.io](https://cronitor.io/) - Cron işleri, web siteleri, API'ler ve daha fazlası için performans bilgileri ve çalışma süresi izleme. Beş monitörlü ücretsiz bir katman.
  * [datadoghq.com](https://www.datadoghq.com/) - 5 düğüme kadar ücretsiz
  * [deadmanssnitch.com](https://deadmanssnitch.com/) - Cron işlerini izleme. Bir ücretsiz muhbir (monitör), başkalarını kaydolmaya yönlendirirseniz daha fazlası
  * [downtimemonkey.com](https://downtimemonkey.com/) - 60 çalışma süresi monitörü, 5 dakikalık aralık. E-posta, Slack uyarıları.
  * [economize.cloud](https://economize.cloud) - Ekonomileştirme, bulut kaynaklarını optimize edecek ve raporlayacak şekilde düzenleyerek bulut altyapısı maliyetlerinin anlaşılmasına yardımcı olur. Her ay Google Cloud Platform'da harcanan 5.000 ABD dolarına kadar ücretsiz.
  * [fivenines.io](https://fivenines.io/) - Gerçek zamanlı kontrol panelleri ve uyarılarla Linux sunucu izleme - 60 saniye aralıklarla 5'e kadar izlenen sunucu için sonsuza kadar ücretsiz. Kredi kartı gerekmez.
  * [FlareWarden](https://flarewarden.com) - Çoklu bölge doğrulama ve durum sayfalarıyla çalışma süresi, içerik, bağımlılık ve SSL izleme. Ücretsiz planda 15 monitör, 5 dakikalık kontrol ve 90 günlük geçmiş bulunur.
  * [Grafana Cloud](https://grafana.com/products/cloud/) - Grafana Cloud, ölçümleri ve günlükleri Grafana ile entegre eden, şekillendirilebilir bir gözlemlenebilirlik platformudur. Ücretsiz: 3 kullanıcı, on kontrol paneli, 100 uyarı, Prometheus ve Graphite'te metrik depolama (10.000 seri, 14 gün saklama), Loki'de günlük depolama (50 GB günlük, 14 gün saklama)
  * [healthchecks.io](https://healthchecks.io) - Cron işlerinizi ve arka plan görevlerinizi izleyin. 20 çeke kadar ücretsiz.
  * [incidenthub.cloud](https://incidenthub.cloud/) - Bulut ve SaaS durum sayfası toplayıcı - 20 monitör ve 2 bildirim kanalı (Slack ve Discord) sonsuza kadar ücretsizdir.
  * [inspector.dev](https://www.inspector.dev) - Sonsuza kadar ücretsiz katmanla bir dakikadan kısa sürede eksiksiz bir Gerçek Zamanlı izleme kontrol paneli.
  * [instatus.com](https://instatus.com) - 10 saniye içinde güzel bir durum sayfasına sahip olun. Sınırsız abonelik ve sınırsız ekiple sonsuza kadar ücretsiz.
  * [linkok.com](https://linkok.com) - Çevrimiçi bozuk bağlantı denetleyicisi, 100 sayfaya kadar küçük web siteleri için ücretsiz, açık kaynaklı projeler için tamamen ücretsiz.
  * [loader.io](https://loader.io/) - Sınırlamalara sahip ücretsiz yük testi araçları
  * [Middleware.io](https://middleware.io/) - Ara yazılım gözlemlenebilirlik platformu, uygulamalarınız ve yığınınız için tam görünürlük sağlar, böylece sorunları geniş ölçekte izleyebilir ve teşhis edebilirsiniz. Geliştirici topluluğunun kullanımına yönelik, 1 milyona kadar günlük olayı için Günlük izleme, 2 ana bilgisayara kadar Altyapı izleme ve APM'ye olanak tanıyan, sonsuza kadar ücretsiz bir plana sahiptirler.
  * [MonitorMonk](https://monitormonk.com) - Güzel durum sayfalarıyla minimalist çalışma süresi izleme. Forever Free planı, 10 web sitesi veya API uç noktası için HTTPS, Anahtar Kelime, SSL ve Yanıt Süresi izleme olanağı sunar ve 2 kontrol paneli/durum sayfası sağlar.
  * [netdata.cloud](https://www.netdata.cloud/) - Netdata, gerçek zamanlı ölçümleri toplamak için kullanılan açık kaynaklı bir araçtır. Büyüyen bir üründür ve GitHub'da da bulunabilir!
  * [newrelic.com](https://www.newrelic.com) - Mühendislerin daha mükemmel yazılım oluşturmasına yardımcı olmak için oluşturulmuş yeni Relic gözlemlenebilirlik platformu. Monolitlerden sunucusuz yazılımlara kadar her şeyi ölçebilir ve ardından tüm yazılım yığınınızı analiz edebilir, sorun giderebilir ve optimize edebilirsiniz. Ücretsiz katman, ayda 100 GB ücretsiz veri alımı, bir ücretsiz tam erişimli kullanıcı ve sınırsız ücretsiz birincil kullanıcı sunar.
  * [OnlineOrNot.com](https://onlineornot.com/) - OnlineOrNot, web siteleri ve API'ler için çalışma süresi izleme, cron işleri ve zamanlanmış görevler için izleme sağlar. Ayrıca durum sayfaları da sağlar. 3 dakika ara ile ilk 5 kontrol ücretsizdir. Ücretsiz katman, uyarıları Slack, Discord ve E-posta yoluyla gönderir.
  * [OntarioNet.ca CN Testi](https://cntest.ontarionet.ca) - Bir web sitesinin Çin'de Büyük Güvenlik Duvarı tarafından engellenip engellenmediğini kontrol edin. Çin'deki sunucular tarafından tespit edilen DNS sonuçlarını ve ASN bilgilerini ABD'deki sunucularla karşılaştırarak DNS kirliliğini tanımlar.
  * [pagecrawl.io](https://pagecrawl.io/) - Günlük kontrollerle 6 monitöre kadar ücretsiz olarak web sitesi değişikliklerini izleyin.
  * [pagertree.com](https://pagertree.com/) - Uyarı ve çağrı yönetimi için basit arayüz. 5 kullanıcıya kadar ücretsiz.
  * [phare.io](https://phare.io/) - Sınırsız proje ve sınırsız durum sayfası için 100.000'e kadar olay için ücretsiz Çalışma Süresi İzleme.
  * [pingbreak.com](https://pingbreak.com/) - Modern çalışma süresi izleme hizmeti. Sınırsız URL'yi kontrol edin ve Discord, Slack veya e-posta yoluyla kesinti bildirimleri alın.
  * [Pingmeter.com](https://pingmeter.com/) - 10 dakikalık aralıklarla 5 çalışma süresi monitörü. SSH, HTTP, HTTPS ve tüm özel TCP bağlantı noktalarını izleyin.
  * [pingpong.one](https://pingpong.one/) - İzleme özellikli gelişmiş durum sayfası platformu. Ücretsiz katman, SSL alt alan adına sahip, herkese açık, özelleştirilebilir bir durum sayfası içerir. Pro plan, açık kaynaklı projelere ve kar amacı gütmeyen kuruluşlara ücretsiz olarak sunulmaktadır.
  * [Pulsetic](https://pulsetic.com) - 10 monitör, 6 Aylık geçmiş Çalışma Süresi/Günlükler, sınırsız durum sayfaları ve özel alanlar dahildir! Sonsuz süre ve ücretsiz sınırsız e-posta uyarıları için. Kredi kartına ihtiyacınız yok.
  * [robusta.dev](https://home.robusta.dev/) - Prometheus'u temel alan güçlü Kubernetes izleme. Kendi Prometheus'unuzu getirin veya hepsi bir arada paketi kurun. Ücretsiz katmanda en fazla 20 Kubernetes düğümü bulunur. Slack, Microsoft Teams, Discord ve daha fazlası aracılığıyla uyarılar. PagerDuty, OpsGenie, VictorOps, DataDog ve diğer birçok araçla entegrasyonlar.
  * [Servervana](https://servervana.com) - Büyük projelere ve ekiplere yönelik destekle gelişmiş çalışma süresi izleme. HTTP izleme, Tarayıcı tabanlı izleme, DNS izleme, etki alanı izleme, durum sayfaları ve daha fazlasını sağlar. Ücretsiz katmanda 10 HTTP monitörü, 1 DNS monitörü ve bir durum sayfası bulunur.
  * [Basit Gözlemlenebilirlik](https://simpleobservability.com) - Kurulum karmaşıklığı olmadan, ölçümler ve günlükler için birleşik bir platformda güçlü sunucu izleme. Bir sunucu için ücretsiz.
  * [sitesure.net](https://sitesure.net) - Web sitesi ve cron izleme - 2 monitör ücretsiz
  * [skylight.io](https://www.skylight.io/) - İlk 100.000 istek için ücretsiz (Yalnızca Rails)
  * [statthat.com](https://www.stathat.com/) - On istatistikle ücretsiz başlayın, süre sonu yok
  * [statuscake.com](https://www.statuscake.com/) - Web sitesi izleme, sınırlamalarla birlikte ücretsiz sınırsız testler
  * [statusgator.com](https://statusgator.com/) - Durum sayfası izleme, 3 monitör ücretsiz
  * [supaguard.app](https://supaguard.app/) - 20'den fazla küresel bölgeden sentetik izleme. Ücretsiz katman, yapay zeka destekli kendi kendini iyileştirme ve otomatik test oluşturma özellikleriyle ayda 1.000 tarayıcı kontrolü içerir.
  * [SweetUptime](https://dicloud.net/sweetuptime-server-uptime-monitoring/) - Sunucu izleme, çalışma süresi izleme, DNS ve etki alanı izleme. 10 sunucuyu, 10 çalışma süresini ve 10 alanı ücretsiz izleyin.
  * [syagent.com](https://syagent.com/) - Ticari olmayan ücretsiz sunucu izleme hizmeti, uyarılar ve ölçümler.
  * [UptimeObserver.com](https://uptimeobserver.com) - Ticari kullanım için bile olsa, 5 dakikalık aralıklarla 20 çalışma süresi monitörü ve özelleştirilebilir bir durum sayfası edinin. E-posta ve Telegram yoluyla sınırsız, gerçek zamanlı bildirimlerin keyfini çıkarın. Başlamak için kredi kartına gerek yok.
  * [uptimetoolbox.com](https://uptimetoolbox.com/) - Beş web sitesi için ücretsiz izleme, 3 dakikalık aralıklarla, genel durum sayfası.
  * [Wachete](https://www.wachete.com) - beş sayfayı izler, 24 saatte bir kontrol eder.
  * [Xitoring.com](https://xitoring.com/) - Çalışma süresi izleme: 20 ücretsiz, Linux ve Windows Sunucu izleme: 5 ücretsiz, Durum sayfası: 1 ücretsiz - Mobil uygulama, çoklu bildirim kanalı ve çok daha fazlası!

**[⬆️Başa Dön](#table-of-contents)**

## Crash and Exception Handling

  * [Axiom](https://axiom.co/) - 30 günlük saklama süresiyle 0,5 TB'a kadar günlük depolayın. Vercel gibi platformlarla entegrasyonları ve e-posta/Discord bildirimleriyle gelişmiş veri sorgulamayı içerir.
  * [Bugsink](https://www.bugsink.com/) - Sentry-SDK uyumluluğuyla hata izleme. Ayda 5.000'e kadar hata için ücretsiz veya kendi kendine barındırıldığında sınırsız kullanım.
  * [bugsnag.com](https://www.bugsnag.com/) - İlk denemeden sonra ayda 2.000 hataya kadar ücretsiz
  * [CatchJS.com](https://catchjs.com/) - Ekran görüntüleri ve tıklama izleriyle JavaScript hata takibi. Açık kaynaklı projeler için ücretsizdir.
  * [elmah.io](https://elmah.io/) - Web geliştiricileri için hata günlüğü tutma ve çalışma süresini izleme. Açık kaynaklı projeler için ücretsiz Small Business aboneliği.
  * [Kucakla](https://embrace.io/) - Mobil uygulama izleme. Yılda 1 milyona kadar kullanıcı oturumu olan küçük ekipler için ücretsizdir.
  * [istisnasız](https://exceptionless.com) - Gerçek zamanlı hata, özellik, günlük raporlama ve daha fazlası. Ayda 3 bin etkinlik/1 kullanıcı için ücretsiz. Açık kaynaktır ve sınırsız kullanım için kendi kendine barındırılması kolaydır.
  * [GlitchTip](https://glitchtip.com/) - Basit, açık kaynaklı hata izleme. Açık kaynaklı Sentry SDK'larıyla uyumludur. Ayda 1000 etkinlik ücretsiz veya sınırsız olarak kendi kendine barındırılabilir
  * [honeybadger.io](https://www.honeybadger.io) - İstisna, çalışma süresi ve cron izleme. Küçük ekipler ve açık kaynaklı projeler için ücretsiz (ayda 12.000 hata).
  * [Jam](https://jam.dev) - Tek tıklamayla geliştirici dostu hata raporları. Sınırsız reçel içeren ücretsiz plan.
  * [memfault.com](https://memfault.com) - Bulut cihazı gözlemlenebilirliği ve hata ayıklama platformu. [Nordic](https://app.memfault.com/register-nordic), [NXP](https://app.memfault.com/register-nxp) ve [Laird](https://app.memfault.com/register-laird) cihazları için 100 cihaz ücretsiz.
  * [rollbar.com](https://rollbar.com/) - İstisna ve hata izleme, ayda 5.000 hata içeren ücretsiz plan, sınırsız kullanıcı, 30 gün saklama
  * [Semaphr](https://semaphr.com) - Mobil uygulamalarınız için ücretsiz hepsi bir arada kapatma anahtarı.
  * [sentry.io](https://sentry.io/) - Sentry, uygulama istisnalarını gerçek zamanlı olarak izler ve küçük bir ücretsiz planı vardır. Aylık 5.000 hata/1 kullanıcı için ücretsiz, kendi kendine barındırılıyorsa sınırsız kullanım
  * [Whitespace](https://whitespace.dev) - Tek tıklamayla hata raporları doğrudan tarayıcınızda. Kişisel kullanım için sınırsız kayıt içeren ücretsiz plan.

**[⬆️Başa Dön](#table-of-contents)**

## Search

  * [algolia.com](https://www.algolia.com/) - Kolayca arama deneyimleri oluşturmak için yazım hatası toleransı, alaka düzeyi ve kullanıcı arayüzü kitaplıkları ile barındırılan arama çözümü. Ücretsiz "Derleme" planı ayda 1 milyon belge ve 10 bin arama içerir. Ayrıca ücretsiz olarak [geliştirici dokümantasyonu araması](https://docsearch.algolia.com/) olanağı sunar.
  * [bonsai.io](https://bonsai.io/) - Ücretsiz 1 GB bellek ve 1 GB depolama alanı
  * [CommandBar](https://www.commandbar.com/) - Kullanıcılarınızın ürününüz içindeki içerikleri, gezinmeleri, özellikleri vb. aramasına olanak tanıyan ve keşfedilebilirliğe yardımcı olan hizmet olarak Birleşik Arama Çubuğu, web tabanlı kullanıcı arayüzü widget'ı/eklentisi. 1.000 Aylık Aktif Kullanıcıya kadar ücretsiz, sınırsız komut.
  * [searchly.com](http://www.searchly.com/) - Ücretsiz 2 dizin ve 20 MB depolama alanı

**[⬆️Başa Dön](#table-of-contents)**

## Education and Career Development

  * [Cisco Ağ Akademisi, Herkes için Beceriler](https://skillsforall.com/) - Siber güvenlik, ağ iletişimi ve Python gibi konularda sertifikaya uygun ücretsiz kurslar sunar.
  * [DeepLearning.AI Kısa Kursları](https://www.deeplearning.ai/short-courses/) - Bir saat veya daha kısa sürede en yeni üretken AI araçları ve teknikleriyle uygulamalı deneyim elde etmek için sektör lideri uzmanlardan ücretsiz kısa kurslar.
  * [DevNet Academy](https://devnet-academy.com/) - Cisco DevNet Expert / CCIE Automation sertifikasyonu için ücretsiz, temposunu kendiniz belirleyebileceğiniz eğitim. Python Click ve Flask-RESTx'i kapsar.
  * [Django-tutorial.dev](https://django-tutorial.dev) - İlk çerçeveleri olarak Django'yu öğrenmek için ücretsiz çevrimiçi kılavuzlar ve kullanıcılar tarafından yazılan makalelere ücretsiz dofollow geri bağlantısı sağlar.
  * [edX](https://www.edx.org/) - Harvard ve MIT dahil olmak üzere bilgisayar bilimi, mühendislik ve veri bilimi alanlarında uzmanlaşmış 250 önde gelen kurumdan 4.000'den fazla ücretsiz çevrimiçi kursa erişim sunar.
  * [Egzersiz](https://exercism.org) - 75'ten fazla programlama dilinde, insan danışmanlığıyla ücretsiz, açık kaynaklı programlama eğitimi. Kâr amacı gütmeyen bir kuruluş.
  * [Ücretsiz Profesyonel Özgeçmiş Şablonları ve Düzenleyici](https://www.overleaf.com/latex/templates/tagged/cv) - Deneyimli Profesyonellerin çok sayıda Özgeçmiş şablonunu içeren, tamamen klonlamaya, düzenlemeye ve indirmeye hazır, ATS optimize edilmiş ücretsiz platform.
  * [FreeCodeCamp](https://www.freecodecamp.org/) - Veri Analizi, Bilgi Güvenliği, Web Geliştirme ve daha birçok alanda ücretsiz kurslar ve sertifikalar sunan açık kaynaklı platform.
  * [Full Stack Open](https://fullstackopen.com/en/) - React, Node.js, GraphQL, TypeScript ve daha fazlasıyla modern web geliştirme üzerine üniversite düzeyinde ücretsiz kurs. Tamamen çevrimiçi ve kendi hızınızda.
  * [Etkileşimli CV](https://interactive-cv.com) - Gerçek zamanlı düzenleme ve ATS optimizasyonuna sahip yapay zeka destekli özgeçmiş oluşturucu. Ücretsiz katman, premium şablonlara (Harvard, Europass) otomatik CV dönüştürmeyi, PDF dışa aktarmayı, sınırsız iş ilanı bilgilerine sahip iş takibini ve sohbet/ses özellikleriyle CV paylaşımını içerir.
  * [Khan Academy](https://www.khanacademy.org/computing/computer-programming) - Temel ve ileri düzey HTML/CSS, JavaScript ve SQL öğrenmek için ücretsiz çevrimiçi kılavuzlar.
  * [LabEx](https://labex.io) - Etkileşimli laboratuvarlar ve gerçek dünya projeleri aracılığıyla Linux, DevOps, Siber Güvenlik, Programlama, Veri Bilimi ve daha pek çok alanda becerilerinizi geliştirin.
  * [MIT OpenCourseWare](https://ocw.mit.edu/) - MIT OpenCourseWare, 2.500'den fazla MIT kursundan alınan materyallerin çevrimiçi bir yayınıdır ve bilgileri dünya çapındaki öğrenciler ve eğitimcilerle özgürce paylaşır. Youtube kanalını şu adreste bulabilirsiniz: [@mitocw](https://www.youtube.com/@mitocw/featured)
  * [Roadmap.sh](https://roadmap.sh) - Blockchain'den UX Tasarımına kadar geliştirmenin tüm yönlerini kapsayan ücretsiz öğrenme yol haritaları.
  * [Odin Projesi](https://www.theodinproject.com/) - Web geliştirme için JavaScript ve Ruby'ye odaklanan bir müfredata sahip ücretsiz, açık kaynaklı platform.
  * [W3Schools](https://www.w3schools.com/) - HTML, CSS, JavaScript ve daha fazlası gibi web geliştirme teknolojileri hakkında ücretsiz eğitimler sunar.

**[⬆️Başa Dön](#table-of-contents)**

## Email

  * [10minutemail](https://10minutemail.com) - Test için ücretsiz, geçici e-posta.
  * [AhaSend](https://ahasend.com) - Ücretsiz planda sınırsız alan adları, ekip üyeleri, web kancaları ve mesaj rotaları içeren, ayda 1000 e-posta için ücretsiz, işlemsel e-posta hizmeti.
  * [AnonAddy](https://anonaddy.com) - Açık kaynaklı anonim e-posta yönlendirme, ücretsiz olarak sınırsız e-posta takma adı oluşturma
  * [Antideo](https://www.antideo.com) - Ücretsiz katmanda e-posta doğrulaması, IP ve telefon numarası doğrulaması için saat başına 10 API isteği. Kredi Kartına gerek yoktur.
  * [Brevo](https://www.brevo.com/) - 9.000 e-posta/ay, 300 e-posta/gün ücretsiz
  * [Bump](https://bump.email/) - Ücretsiz 10 Bump e-posta adresi, bir özel alan adı
  * [Burnermail](https://burnermail.io/) - Ücretsiz 5 Burner E-posta Adresi, 1 Posta Kutusu, 7 Günlük Posta Kutusu Geçmişi
  * [Buttondown](https://buttondown.email/) - Haber bülteni hizmeti. 100 aboneye kadar ücretsiz
  * [Contact.do](https://contact.do/) - Bağlantıdaki iletişim formu (iletişim formları için biraz)
  * [debugmail.io](https://debugmail.io/) - Geliştiriciler için kullanımı kolay test posta sunucusu
  * [dkimvalidator.com](https://dkimvalidator.com/) - E-postanın DNS/SPF/DKIM/DMARC ayarlarının doğru olup olmadığını test edin, roundsphere.com'dan ücretsiz hizmet
  * [DNSExit](https://dnsexit.com/) - 100 MB depolama alanıyla birlikte alanınız altında en fazla 2 E-posta adresi ücretsiz. IMAP, POP3, SMTP, SPF/DKIM desteği.
  * [EmailGuard](https://emailguard.lazrek.net/) - Basit bir API aracılığıyla tek kullanımlık e-postaları engelleyin, yazım hatalarını yakalayın ve MX kayıtlarını doğrulayın. Ayda 100 ücretsiz istek.
  * [EmailJS](https://www.emailjs.com/) - Bu, e-posta sunucusunun tamamı değil; bu yalnızca, kimlik bilgilerinizi açığa vurmadan doğrudan istemciden e-posta göndermek için kullanabileceğiniz bir e-posta istemcisidir, ücretsiz katmanda 200 aylık istek, 2 e-posta şablonu, 50Kb'a kadar istekler, Sınırlı iletişim geçmişi bulunur.
  * [EmailLabs.io](https://emaillabs.io/en) - Her ay 9.000'e kadar E-postayı, günde 300'e kadar e-postayı ücretsiz gönderin.
  * [EmailOctopus](https://emailoctopus.com) - Ayda 2.500 aboneye ve 10.000 e-postaya kadar ücretsiz
  * [Emailvalidation.io](https://emailvalidation.io) - Ayda 100 ücretsiz e-posta doğrulaması
  * [EtherealMail](https://ethereal.email) - Ethereal, esas olarak Nodemailer ve EmailEngine kullanıcılarını hedefleyen (ancak bunlarla sınırlı olmayan) sahte bir SMTP hizmetidir. Mesajların hiçbir zaman teslim edilmediği, tamamen ücretsiz, işlem karşıtı bir e-posta hizmetidir.
  * [forwardemail.net](https://forwardemail.net) - Özel alan adları için ücretsiz e-posta yönlendirme. Alan adınızla sınırsız sayıda e-posta adresi oluşturun ve iletin (**not**: Spam nedeniyle .casa, .cf, .click, .email, .fit, .ga, .gdn, .gq, .lat, .loan, .london, .men, .ml, .pl, .rest, .ru, .tk, .top, .work TLD'leri kullanıyorsanız ödeme yapmanız gerekir)
  * [E-postayı Taklit Et](https://imitate.email) - Build/qa ve ci/cd genelinde e-posta işlevselliğini test etmek için Korumalı Alan E-posta Sunucusu. Ücretsiz hesaplar sonsuza kadar günde 15 e-posta alır.
  * [ImprovMX](https://improvmx.com) - Ücretsiz e-posta yönlendirme.
  * [Gelen Kutuları Uygulaması](https://inboxesapp.com) - Günde en fazla 3 geçici e-posta oluşturun ve işiniz bittiğinde kullanışlı bir Chrome uzantısından bunları silin. Kayıt akışlarını test etmek için mükemmeldir.
  * [inboxkitten.com](https://inboxkitten.com/) - 3 güne kadar e-postaların otomatik olarak silindiği ücretsiz geçici/tek kullanımlık e-posta gelen kutusu. Açık kaynaktır ve kendi kendine barındırılabilir.
  * [mail-tester.com](https://www.mail-tester.com) - E-postanın DNS/SPF/DKIM/DMARC ayarlarının doğru olup olmadığını test edin, ayda 20 ücretsiz.
  * [Maileroo](https://maileroo.com) - Geliştiriciler için SMTP geçişi ve e-posta API'si. Ayda 5.000 e-posta, sınırsız alan adı, ücretsiz e-posta doğrulama, kara liste izleme, posta test aracı ve daha fazlası.
  * [mailcatcher.me](https://mailcatcher.me/) - Postaları yakalar ve bir web arayüzü aracılığıyla sunar.
  * [mailchannels.com](https://www.mailchannels.com) - REST API ve SMTP entegrasyonlarına sahip e-posta API'si, ayda 3.000 e-postaya kadar ücretsizdir.
  * [Mailcheck.ai](https://www.mailcheck.ai/) - Kullanıcıların geçici e-posta adresleriyle kaydolmasını önleyin, saatte 120 istek (~86.400 aylık)
  * [Maildroppa](https://maildroppa.com) - 100'e kadar abone ve sınırsız e-postanın yanı sıra ücretsiz otomasyonlar.
  * [MailerLite.com](https://www.mailerlite.com) - 1.000 abone/ay, 12.000 e-posta/ay ücretsiz
  * [MailerSend.com](https://www.mailersend.com) - E-posta API'si, SMTP, işlemsel e-postalar için ayda 3.000 e-posta ücretsiz
  * [mailinator.com](https://www.mailinator.com/) - İstediğiniz gelen kutusunu kullanabileceğiniz ücretsiz, genel e-posta sistemi
  * [Mailjet](https://www.mailjet.com/) - 6.000 e-posta/ay ücretsiz (günlük 200 e-posta gönderme sınırı)
  * [mailsac.com](https://mailsac.com) - Geçici e-posta testi için ücretsiz API, ücretsiz genel e-posta barındırma, giden yakalama, slack/websocket/webhook'a e-posta (1.500 aylık API sınırı)
  * [Mailtrap.io](https://mailtrap.io/) - E-posta API'si, SMTP, işlem ve pazarlama e-postaları için ayda 3.500 e-posta ücretsiz. E-posta Korumalı Alanı - geliştirme için sahte SMTP sunucusu, bir gelen kutusuyla ücretsiz plan, 100 mesaj, ekip üyesi yok, saniyede iki e-posta, iletme kuralı yok.
  * [Mutant Mail](https://www.mutantmail.com/) - Ücretsiz 10 E-posta Kimliği, 1 Alan Adı, 1 Posta Kutusu. Tüm E-posta Kimlikleri için Tek Posta Kutusu.
  * [OneSignal](https://onesignal.com/) - 10.000 e-posta/ay,Kredi Kartı gerekmez.
  * [Parsio.io](https://parsio.io) - Ücretsiz e-posta ayrıştırıcı (E-postayı iletin, verileri çıkarın, sunucunuza gönderin)
  * [Plunk](https://useplunk.com) - Ayda 3 bin e-posta ücretsiz
  * [Postmark](https://postmarkapp.com/) - Ayda 100 e-posta ücretsiz, sınırsız haftalık DMARC özeti.
  * [Proton Mail](https://proton.me/mail) - Yerleşik uçtan uca şifrelemeye sahip ücretsiz güvenli e-posta hesabı servis sağlayıcısı. Ücretsiz 1 GB depolama alanı.
  * [Yeniden Gönder](https://resend.com) - Geliştiriciler için işlemsel e-posta API'si. Ayda 3.000 e-posta, günde 100 e-posta ücretsiz, bir özel alan adı.
  * [Gönderen](https://www.sender.net) - Ayda 15.000'e kadar e-posta, 2.500'e kadar abone
  * [Sendpulse](https://sendpulse.com) - 500 abone/ay, 15.000 e-posta/ay ücretsiz
  * [SendStreak](https://www.sendstreak.com/) - Kendi SMTP sunucunuza (ör. AWS, Maileroo, Gmail) şablonlar, otomasyonlar, geçmiş vb. ekleyen bir hizmet olarak e-posta çerçevesi. Günde 100 e-postaya kadar ücretsiz, süre sınırı yok.
  * [SimpleLogin](https://simplelogin.io/) - Açık kaynak, kendi kendine barındırılabilen e-posta takma adı/yönlendirme çözümü. Ücretsiz 10 Takma Ad, sınırsız bant genişliği, sınırsız yanıtlama/gönderme. Eğitim personeli (öğrenci, araştırmacı vb.) için ücretsizdir.
  * [Substack](https://substack.com) - Sınırsız ücretsiz bülten hizmeti. Ücretlendirdiğinizde ödemeye başlayın.
  * [Sweego](https://www.sweego.io/) - Geliştiriciler için Avrupa işlemsel e-posta API'si. Günde 100 e-posta ücretsiz.
  * [temp-mail.io](https://temp-mail.io) - Aynı anda birden fazla e-posta gönderme ve yönlendirme içeren ücretsiz tek kullanımlık geçici e-posta hizmeti
  * [Temp-Mail.org](https://temp-mail.org/en/) - Geçici / Tek Kullanımlık Posta Oluşturma Çeşitli alan adlarından yararlanır. E-posta Adresi her zaman yenilenir, sayfa yeniden yüklenir. Tamamen ücretsizdir ve hizmetlerine ilişkin herhangi bir fiyatlandırma içermez.
  * [TempMailDetector.com](https://tempmaildetector.com/) - Ayda 200'e kadar e-postayı ücretsiz olarak doğrulayın ve bir e-postanın geçici olup olmadığını görün.
  * [trashmail.com](https://www.trashmail.com) - Yönlendirme ve otomatik adres geçerlilik süresinin sona ermesiyle ücretsiz tek kullanımlık e-posta adresleri
  * [Tuta](https://tuta.com/) - Yerleşik uçtan uca şifrelemeye sahip, reklamsız, izlemesiz, ücretsiz güvenli e-posta hesabı servis sağlayıcısı. Ücretsiz 1 GB depolama alanı, bir takvim (Tuta'nın ayrıca bir [ücretli planı](https://tuta.com/pricing) var.). Tuta ayrıca kısmen [açık kaynaktır](https://github.com/tutao/tutanota), dolayısıyla kendi sunucunuzu barındırabilirsiniz.
  * [Verifalia](https://verifalia.com/email-verification-api) - Posta kutusu onayı ve tek kullanımlık e-posta adresi algılayıcısı ile gerçek zamanlı e-posta doğrulama API'si; Günde 25 ücretsiz e-posta doğrulaması.
  * [verimail.io](https://verimail.io/) - Toplu ve API e-posta doğrulama hizmeti. Ayda 100 ücretsiz doğrulama
  * [Waitlio](https://waitlio.com/) - Ürün lansmanları için bekleme listesi yönetim yazılımı. Markalı bekleme listesi sayfaları oluşturun, e-posta abonelerini toplayın ve doğrulayın, kayıt işlemlerini etiketler ve analizlerle yönetin. Ücretsiz plan ayda 100 abone, 1 bekleme listesi ve API erişimi içerir.
  * [Sarmalar](https://wraps.dev) - e-posta otomasyonu iş akışları, 5 bin izlenen etkinlik ve sınırsız kişi ücretsiz.

**[⬆️Başa Dön](#table-of-contents)**

## Feature Toggles Management Platforms

  * [Abby](https://www.tryabby.com) - Açık Kaynak özellik işaretleri ve A/B testleri. Kod ve Tamamen Yazılan TypeScript SDK'ları Olarak Yapılandırma. Next.js ve React gibi Çerçevelerle güçlü entegrasyon. Cömert ücretsiz katman ve ucuz ölçeklendirme seçenekleri.
  * [ConfigCat](https://configcat.com) - ConfigCat, sınırsız ekip boyutuna, mükemmel desteğe ve makul bir fiyat etiketine sahip, geliştirici merkezli bir özellik işaretleme hizmetidir. 10'a kadar bayrak, iki ortam, 1 ürün ve ayda 5 Milyon isteğe kadar ücretsiz plan.
  * [Flagsmith](https://flagsmith.com) - Özellikleri güvenle yayınlayın; web, mobil ve sunucu tarafı uygulamalardaki özellik işaretlerini yönetin. Barındırılan API'mizi kullanın, kendi özel bulutunuza dağıtın veya şirket içinde çalıştırın.
  * [GrowthBook](https://growthbook.io) - Yerleşik Bayes istatistiksel analiz motoruna sahip açık kaynak özellik işareti ve A/B testi sağlayıcısı. 3 kullanıcıya kadar ücretsiz, sınırsız özellik işaretleri ve deneyler.
  * [Hypertune](https://www.hypertune.com) - Git tarzı sürüm kontrolü ve eşzamanlı, bellek içi, yerel işaret değerlendirmesi ile tür açısından güvenli özellik işaretleri, A/B testi, analizler ve uygulama yapılandırması. Sınırsız özellik işaretleri ve A/B testleri ile en fazla 5 ekip üyesi için ücretsiz.
  * [Statsig](https://www.statsig.com) - Özellik yönetimi, A/B testi, analiz ve daha fazlası için güçlü bir platform. Cömert ücretsiz planı, ayda 1 milyona kadar etkinliği destekleyen sınırsız koltuk, bayrak, deney ve dinamik konfigürasyonlar sunar.
  * [Toggled.dev](https://www.toggled.dev) - Kurumsal kullanıma hazır, ölçeklenebilir çok bölgeli özellik, yönetim platformunu değiştirir. 10'a kadar bayrak, iki ortam, sınırsız istek içeren ücretsiz plan. SDK, analiz panosu, sürüm takvimi, Slack bildirimleri ve diğer tüm özellikler sonsuz ücretsiz plana dahildir.


**[⬆️Başa Dön](#table-of-contents)**

## Font

  * [Befonts](https://befonts.com/) - Kişisel veya ticari kullanım için çeşitli benzersiz yazı tipleri sağlar.
  * [Bunny](https://fonts.bunny.net) - Gizlilik odaklı Google Yazı Tipleri
  * [dafont](https://www.dafont.com/) - Bu web sitesinde sunulan yazı tipleri yazarlarının mülkiyetindedir ve ücretsiz yazılım, paylaşılan yazılım, demo sürümleri veya kamu malıdır.
  * [Her Şey Yazı Tipleri](https://everythingfonts.com/) - Birden fazla araç sunar; @font-face, Birim Dönüştürücü, Yazı Tipi Hinter ve Yazı Tipi Gönderen.
  * [Web yazı tipi](https://fontofweb.com/) - Bir web sitesinde kullanılan tüm yazı tiplerini ve bunların nasıl kullanıldığını tanımlayın.
  * [Font Squirrel](https://www.fontsquirrel.com/) - Ticari çalışma için lisanslanan ücretsiz yazı tipleri. Bu yazı tiplerini elle seçip kullanımı kolay bir formatta sunduk.
  * [FontGet](https://www.fontget.com/) - İndirilebilecek çeşitli yazı tipleri vardır ve etiketlerle düzgün bir şekilde sıralanır.
  * [fonts.xz.style](https://fonts.xz.style/) - web sitelerine yazı tipi aileleri sunmak için ücretsiz ve açık kaynaklı hizmet
CSS kullanarak.
  * [Fontsensei](https://fontsensei.com/) - Kullanıcılar tarafından etiketlenen açık kaynaklı Google yazı tipleri. CJK ile (Çince, Japonca,
Korece) yazı tipi etiketleri.
  * [Fontshare](https://www.fontshare.com/) - ücretsiz bir yazı tipi hizmetidir. Kişisel ve ticari kullanım için %100 ücretsiz, giderek büyüyen profesyonel kalitede yazı tipleri koleksiyonudur.
  * [Google Yazı Tipleri](https://fonts.google.com/) - Birçok ücretsiz yazı tipinin, indirme yoluyla veya Google'ın CDN'sine bağlantı yoluyla bir web sitesine yüklenmesi kolay ve hızlıdır.

**[⬆️Başa Dön](#table-of-contents)**

## Forms

  * [FabForm](https://fabform.io/) - Akıllı geliştiriciler için form arka uç platformu. Ücretsiz plan ayda 250 form gönderimine izin verir. Dost canlısı modern GUI. Google E-Tablolar, Airtable, Slack, Email ve diğerleriyle entegre olur.
  * [Feathery](https://feathery.io) - Güçlü, geliştirici dostu form oluşturucu. Kayıt olma ve oturum açma, kullanıcı katılımı, ödeme akışları, karmaşık finansal uygulamalar ve daha fazlasını oluşturun. Ücretsiz plan, ayda 250'ye kadar gönderime ve beş aktif forma izin verir.
  * [feedback.fish](https://feedback.fish/) - Ücretsiz plan, toplam 25 geri bildirim gönderiminin toplanmasına olanak tanır. Sağlanan React ve Vue bileşenleriyle entegrasyonu kolaydır.
  * [FluidForms](https://fluidforms.ai/) - Yapay zeka odaklı mantığa sahip form oluşturucu ve arka uç. Ücretsiz plan ayda 100 yanıt, sınırsız form (AI tarafından oluşturulan formlar dahil), web kancaları ve yerleştirme içerir.
  * [Form.taxi](https://form.taxi/) - HTML form gönderimleri için uç nokta. Bildirimler, spam engelleyiciler ve GDPR uyumlu veri işleme özellikleriyle. Temel kullanım için ücretsiz plan.
  * [Formcarry.com](https://formcarry.com) - HTTP POST Formu uç noktası, Ücretsiz plan 100 aylık gönderime izin verir.
  * [Formester.com](https://formester.com) - Benzersiz görünümlü formları paylaşın ve web sitenize yerleştirin; oluşturulan form sayısında veya plan tarafından kısıtlanan özelliklerde herhangi bir sınırlama yoktur. Her ay 100'e kadar gönderimi ücretsiz olarak alın.
  * [FormKeep.com](https://www.formkeep.com/) - 50 aylık gönderim, spam koruması, e-posta bildirimi ve HTML'yi dışa aktarabilen sürükle ve bırak tasarımcısıyla sınırsız form. Ek özellikler arasında özel alan kuralları, ekipler ve Google E-Tablolar, Slack, ActiveCampaign ve Zapier entegrasyonları bulunur.
  * [formlets.com](https://formlets.com/) - Çevrimiçi formlar, ayda sınırsız tek sayfalı formlar, ayda 100 gönderim, e-posta bildirimleri.
  * [forms.app](https://forms.app/) - Koşullu mantık, otomatik puan hesaplayıcı ve yapay zeka gibi güçlü özelliklere sahip çevrimiçi formlar oluşturun. Ücretsiz planla 100'e kadar yanıt toplayın, formlarınızı bir web sitesine yerleştirin veya bunları bir bağlantıyla birlikte kullanın.
  * [formspark.io](https://formspark.io/) - Formdan E-postaya hizmeti, ücretsiz plan sınırsız formlara izin verir, ayda 250 gönderim, Müşteri destek ekibi tarafından destek.
  * [Formspree.io](https://formspree.io/) - HTTP POST isteği kullanarak e-posta gönderin. Ücretsiz kullanım, form başına ayda 50 gönderimle sınırlıdır.
  * [Formsubmit.co](https://formsubmit.co/) - HTML formlarınız için kolay form uç noktaları. Sonsuza Kadar Ücretsiz. Kayıt gerekli değildir.
  * [Formware.io](https://formware.io/) - Nasıl kodlanacağını bilmeden saniyeler içinde tamamen duyarlı ve büyüleyici formlar oluşturun ve ücretsiz olarak sınırsız yanıt toplayın!
  * [HeroTofu.com](https://herotofu.com/) - Bot algılama ve şifrelenmiş arşiv ile arka uç oluşturur. Gönderimleri kullanıcı arayüzü aracılığıyla e-postaya, Slack'e veya Zapier'e iletin. Kendi ön uçunuzu kullanın. Sunucu kodu gerekmez. Ücretsiz plan sınırsız form ve ayda 100 gönderim sağlar.
  * [HeyForm.net](https://heyform.net/) - Çevrimiçi form oluşturucuyu sürükleyip bırakın. Ücretsiz katman, sınırsız form oluşturmanıza ve sınırsız gönderim toplamanıza olanak tanır. Önceden oluşturulmuş şablonlar, anti-spam ve 100 MB dosya depolama alanıyla birlikte gelir.
  * [Kwes.io](https://kwes.io/) - Zengin özelliklere sahip form uç noktası. Statik sitelerle harika çalışır. Ücretsiz plan, aylık 50 gönderime kadar 1 web sitesini içerir.
  * [Pageclip](https://pageclip.co/) - Ücretsiz plan bir siteye, bir forma ve 1.000 aylık gönderime izin verir.
  * [SimplePDF.eu](https://simplepdf.eu/embed) - Web sitenize bir PDF düzenleyici yerleştirin ve herhangi bir PDF'yi doldurulabilir bir forma dönüştürün. Ücretsiz plan, PDF başına üç gönderimle sınırsız PDF'ye izin verir.
  * [smartforms.dev](https://smartforms.dev/) - Web siteniz için güçlü ve kolay form arka ucu, sonsuza kadar ücretsiz plan ayda 50 gönderime izin verir, 250 MB dosya depolama, Zapier entegrasyonu, CSV/JSON dışa aktarma, özel yönlendirme, özel yanıt sayfası, Telegram ve Slack bot, tek e-posta bildirimleri.
  * [staticforms.xyz](https://www.staticforms.xyz/) - HTML formlarını herhangi bir sunucu tarafı kodu olmadan kolayca ve ücretsiz olarak entegre edin. Kullanıcı formu gönderdikten sonra kayıtlı adresinize form içeriğini içeren bir e-posta gönderilecektir.
  * [Hayatta Kal](https://survicate.com/) - Tek bir araçla tüm kaynaklardan geri bildirim alın ve takip anketleri gönderin. Yapay zeka ile geri bildirimleri otomatik olarak analiz edin ve içgörüler elde edin. Ücretsiz e-posta, web sitesi, ürün içi veya mobil anketler, AI anket oluşturucu ve 25 aylık yanıt.
  * [Tally.so](https://tally.so/) - Tüm özelliklerin %99'u ücretsizdir. Ücretsiz katman şunları yapmanıza olanak sağlar: sınırsız formlar, sınırsız gönderimler, e-posta bildirimleri, form mantığı, ödeme tahsilatı, dosya yükleme, özel teşekkür sayfası ve çok daha fazlası.
  * [Typeform.com](https://www.typeform.com/) - Web sitelerine güzel tasarlanmış formlar ekleyin.  Ücretsiz plan, form başına yalnızca on alana ve 100 aylık yanıta izin verir.
  * [Vidhook](https://vidhook.io/) - Yüksek yanıt oranlarına sahip keyifli anketleri kullanarak geri bildirim toplayın. Ücretsiz planda 1 aktif anket, anket başına 25 yanıt ve özelleştirilebilir şablonlar bulunur.
  * [WaiverStevie.com](https://waiverstevie.com) - REST API'sine sahip Elektronik İmza platformu. Web kancalarıyla bildirim alabilirsiniz. Ücretsiz plan, imzalı belgelere filigran ekler ancak sınırsız zarf + imzaya izin verir.
  * [Web3Forms](https://web3forms.com) - Statik ve JAMStack Web Siteleri için arka uç kodu yazmadan iletişim formları. Ücretsiz plan, Sınırsız Form, Sınırsız Etki Alanı ve ayda 250 Gönderime izin verir.
  * [Wufoo](https://www.wufoo.com/) - Web sitelerinde kullanılacak hızlı formlar. Ücretsiz planın her ay 100 gönderim sınırı vardır.
  * [FormNX](https://FormNX.com/) - Sınırsız form oluşturun ve ücretsiz olarak sınırsız gönderim elde edin. Profesyonelce oluşturulmuş 1000'den fazla form şablonunu kullanın veya sıfırdan formlar oluşturun. E-posta bildirimleri, form mantığı, ödeme toplama, dosya yükleme, özel teşekkür sayfası ve daha pek çok özellikten yararlanın.

**[⬆️Başa Dön](#table-of-contents)**

## Generative AI

  * [Arize AX](https://arize.com) - Yerleşik Alyx aracısı ile AI mühendislerinin/PM'lerin AI uygulamalarını ve aracılarını değerlendirmesine ve gözlemlemesine yardımcı olan AI mühendislik platformu. Ücretsiz ürün, 25.000 aralık ve ayda 1 GB kullanım hacmi içerir.
  * [Ses Geliştirici](https://voice-clone.org/tools/audio-enhancer) - Doğal ses netliğini korurken gürültüyü ve yankıyı ortadan kaldıran yapay zeka destekli ses geliştirici SaaS. Tamamen Ücretsiz: tek tıklamayla sınırsız geliştirme, oturum açmaya gerek yok, MP3/WAV/FLAC desteği
  * [Braintrust](https://www.braintrustdata.com/) - Yapay Zeka Kuşağı için değerlendirmeler, hızlı oyun alanı ve veri yönetimi. Ücretsiz plan, haftada 1.000'e kadar özel değerlendirme satırı sağlar.
  * [Clair](https://askclair.ai/) - Klinik AI Referansı. Öğrenciler Açık Arama, Klinik Özet, Med İncelemesi, İlaç Etkileşimleri, ICD-10 Kodları ve Yöneticiliği içeren profesyonel araç paketine ücretsiz erişime sahiptir. Ayrıca profesyonel süitin ücretsiz deneme sürümü de mevcuttur.
  * [Comet Opik](https://www.comet.com/site/products/opik/) - Geliştirme ve üretim yaşam döngüleriniz boyunca LLM uygulamalarını değerlendirin, test edin ve gönderin. [#açık kaynak](https://github.com/comet-ml/opik/)
  * [Keywords AI](https://keywordsai.co) - En iyi Yüksek Lisans izleme platformu. 2 satır kodla 200'den fazla LLM'yi çağırmak için tek format. Her ay 10.000 ücretsiz istek ve platform özellikleri için 0$!
  * [Langfuse](https://langfuse.com/) - Ekiplerin LLM uygulamalarında işbirliği içinde hata ayıklamasına, analiz etmesine ve yinelemesine yardımcı olan açık kaynaklı LLM mühendislik platformu. Sonsuza kadar ücretsiz plan, ayda 50.000 gözlemi ve tüm platform özelliklerini içerir. [#açık kaynak](https://github.com/langfuse/langfuse)
  * [Langtrace](https://langtrace.ai) - geliştiricilerin istemleri ve veri kümelerini izlemesine, değerlendirmesine, yönetmesine ve bir LLM uygulamasının performansıyla ilgili sorunları ayıklamasına olanak tanır. Gözlemlenebilirliğe yardımcı olan ve herhangi bir gözlemlenebilirlik istemcisiyle çalışan herhangi bir LLM için açık telemetri standart izleri oluşturur. Ücretsiz plan ayda 50.000 izleme sunuyor.
  * [LangWatch](https://langwatch.ai) - AI ekiplerinin LLM uygulamalarını güvenilirlik, maliyet verimliliği ve performans açısından ölçmesine, izlemesine ve optimize etmesine yardımcı olan bir LLMOps platformu. Güçlü bir DSPy bileşeniyle, GenAI ürünlerine ince ayar yapmak ve üretim yapmak için mühendisler ve teknik olmayan ekipler arasında kusursuz işbirliğine olanak sağlıyoruz. Ücretsiz plan, tüm platform özelliklerini, ayda 1 bin izlemeyi ve 1 iş akışı DSPy iyileştiricisini içerir. [#açık kaynak](https://github.com/langwatch/langwatch)
  * [Lumenfall.ai](https://lumenfall.ai/) - OpenAI uyumlu bir API aracılığıyla önde gelen görüntü oluşturma modellerine birleşik erişim sağlayan AI medya ağ geçidi. Platformun kullanımı sıfır işaretleme ve abonelik ücreti olmadan ücretsizdir. Çoğu model için çıkarım maliyetleri sağlayıcı fiyatı üzerinden faturalandırılır, ancak FLUX.1 [schnell] FP8 kayıtlı kullanıcılar için sınırsız kullanımla sonsuza kadar ücretsiz olarak sunulur. Yerleşik yük devretme ve sağlayıcı esnekliği dahildir.
  * [Mediaworkbench.ai](https://mediaworkbench.ai) - MediaWorkbench.ai, Azure OpenAI, DeepSeek ve Google Gemini modelleri için 100.000 ücretsiz kelime sunarak kullanıcıların kod oluşturma, derin araştırma ve görüntü oluşturmaya yönelik güçlü araçlara erişmesine olanak tanır.
  * [OpenRouter](https://openrouter.ai/models?q=free) - DeepSeek R1, V3, Llama ve Moonshot AI dahil olmak üzere çeşitli ücretsiz AI modelleri sağlar. Bu modeller doğal dil işlemede üstündür ve çeşitli geliştirme ihtiyaçlarına uygundur. Bu modellerin kullanımı ücretsiz olsa da ücret sınırlamalarına tabi olduğunu unutmayın. Ek olarak OpenRouter, daha gelişmiş gereksinimler için Claude, OpenAI, Grok, Gemini ve Nova gibi ücretli modeller sunar.
  * [Othor AI](https://othor.ai/) - Tableau, Power BI ve Looker gibi popüler iş zekası çözümlerine yapay zeka tabanlı hızlı, basit ve güvenli bir alternatif. Othor, dakikalar içinde özel iş zekası çözümleri sunmak için büyük dil modellerinden (LLM'ler) yararlanıyor. Sonsuza Kadar Ücretsiz planı, analitik konusunda herhangi bir sınırlama olmaksızın, bir kullanıcı için beş veri kaynağı bağlantısına sahip bir çalışma alanı sağlar. [#açık kaynak](https://github.com/othorai/othor.ai)
  * [Pollinations.AI](https://pollinations.ai/) - ücretsiz API ile kullanımı kolay, ücretsiz görüntü oluşturma yapay zekası. Hiçbir kayıt veya API anahtarı gerekmez ve bir web sitesine veya iş akışına entegrasyon için çeşitli seçenekler bulunur. [#açık kaynak](https://github.com/pollinations/pollinations)
  * [Portkey](https://portkey.ai/) - Gözlemlenebilirlik paketi ve yapay zeka ağ geçidi içeren Nesil Yapay Zeka uygulamaları için kontrol paneli. Her ay 10.000'e kadar isteği ücretsiz olarak gönderin ve kaydedin.
  * [ReportGPT](https://ReportGPT.app) - Yapay Zeka Destekli Yazma Asistanı. Kendi API anahtarınızı getirdiğiniz sürece platformun tamamı ücretsizdir.
  * [Zenable](https://zenable.io) - Policy as Code ile oluşturulan korkulukları kullanarak şirketinizin kalite ve uyumluluk standartlarını karşılamak için Cursor, Windsurf ve Copilot gibi araçlardan gelen çıktıları anında otomatik olarak düzeltin. Ücretsiz katman, MCP sunucusuna günde 100 araç çağrısını ve GitHub Uygulaması aracılığıyla günde 25 ücretsiz otomatik çekme isteği incelemesini içerir.

**[⬆️Başa Dön](#table-of-contents)**

## CDN and Protection

  * [bootstrapcdn.com](https://www.bootstrapcdn.com/) - bootstrap, bootswatch ve fontawesome.io için CDN
  * [CacheFly](https://portal.cachefly.com/signup/free2023) - Ayda 5 TB'a kadar Ücretsiz CDN trafiği, 19 Çekirdek PoP, 1 Alan Adı ve Evrensel SSL.
  * [cdnjs.com](https://cdnjs.com/) - Basit. Hızlı. Güvenilir. İçerik sunumu en iyi şekilde. cdnjs, Cloudflare tarafından desteklenen, tüm web sitelerinin %11'inden fazlasının güvendiği ücretsiz ve açık kaynaklı bir CDN hizmetidir.
  * [developers.google.com](https://developers.google.com/speed/libraries/) - Google Tarafından Barındırılan Kitaplıklar, en popüler Açık Kaynak JavaScript kitaplıklarına yönelik bir içerik dağıtım ağıdır
  * [Gcore](https://gcorelabs.com/) - Küresel içerik dağıtım ağı, 1 TB ve ayda 1 milyon istek ücretsiz ve
ücretsiz DNS barındırma
  * [jsdelivr.com](https://www.jsdelivr.com/) - Ücretsiz, hızlı ve güvenilir bir açık kaynaklı CDN. Npm, GitHub, WordPress, Deno ve daha fazlasını destekler.
  * [Microsoft Ajax](https://docs.microsoft.com/en-us/aspnet/ajax/cdn/overview) - Microsoft Ajax CDN, jQuery gibi popüler üçüncü taraf JavaScript kitaplıklarını barındırır ve bunları Web uygulamanıza kolayca eklemenizi sağlar
  * [Namecheap Supersonic](https://www.namecheap.com/supersonic-cdn/#free-plan) - Ücretsiz DDoS koruması
  * [ovh.ie](https://www.ovh.ie/ssl-gateway/) - Ücretsiz DDoS koruması ve SSL sertifikası
  * [PromoProxy](https://promoproxy.net/) - Ücretsiz bulut Güvenli Web Ağ Geçidi. Ücretsiz planda en fazla 5 kullanıcı ve günde 1 GB yer alır.
  * [raw.githack.com](https://raw.githack.com/) - Dosyaları Cloudflare kullanarak barındıran **rawgit.com**'un modern bir alternatifi
  * [Skypack](https://www.skypack.dev/) - %100 Yerel ES Modülü JavaScript CDN'si. Alan adı başına aylık 1 milyon istek için ücretsiz.
  * [statically.io](https://statically.io/) - Git depoları (GitHub, GitLab, Bitbucket), WordPress ile ilgili varlıklar ve resimler için CDN
  * [Stellate](https://stellate.co/) - Stellate, GraphQL API'niz için son derece hızlı, güvenilir bir CDN'dir ve iki hizmet için ücretsizdir.
  * [toranproxy.com](https://toranproxy.com/) - Packagist ve GitHub için proxy. CD'yi asla başarısızlığa uğratmayın. Kişisel kullanım için ücretsiz, tek geliştirici, destek yok
  * [UNPKG](https://unpkg.com/) - npm'deki her şey için CDN
  * [weserv](https://images.weserv.nl/) - Bir görüntü önbellek ve yeniden boyutlandırma hizmeti. Dünya çapında bir önbellek ile görüntüleri anında işleyin.

**[⬆️Başa Dön](#table-of-contents)**

## PaaS

  * [ampt.dev](https://getampt.com/) - Ampt, ekiplerin karmaşık yapılandırmalar veya altyapı yönetimi olmadan AWS'de JavaScript uygulamaları oluşturmasına, dağıtmasına ve ölçeklendirmesine olanak tanır. Ücretsiz Önizleme planı saatlik 500 çağrı, günlük 2.500 çağrı ve aylık 50.000 çağrı içerir. Özel alan adlarına yalnızca ücretli planlarda izin verilir.
  * [anvil.works](https://anvil.works) - Python'dan başka hiçbir şey kullanmadan web uygulaması geliştirme. Sınırsız uygulama ve 30 saniyelik zaman aşımına sahip ücretsiz katman.
  * [Apply.build](https://apply.build/) - 0,5 vCPU / 512 MiB RAM, Avrupa sunucuları, otomatik güvenlik duvarı, gerçek zamanlı performans ölçümleriyle GitHub uygulamanızı ücretsiz olarak oluşturun ve dağıtın. Node.js, Python, Go, Java, statik siteler, mikro hizmetler ve daha fazlasını çalıştırın.
  * [appwrite](https://appwrite.io) - Proje duraklatma olmadan (websocket'leri destekler) ve kimlik doğrulama hizmetiyle sınırsız proje. Ücretsiz katmanda proje başına 1 Veritabanı, 3 Paket, 5 İşlev.
  * [Akıllı Bulut](https://clever.cloud) - Otomatik dağıtımlar, otomatik ölçeklendirme, yönetilen veritabanları ve Git tabanlı iş akışlarıyla Avrupa PaaS. Kayıt sırasında 20 € ücretsiz kredi, ücretsiz MySQL ve PostgreSQL veritabanlarını içeren sınırlı bir DEV planı ve Heptapod ve FS Buckets gibi hizmetler için ücretsiz tahsisler içerir.
  * [Choreo](https://wso2.com/choreo/) - Hizmet olarak yapay zekaya özgü dahili geliştirici platformu. Ücretsiz katman, en fazla 5 bileşen ve ayda 100 ABD doları tutarında kredi içerir.
  * [codenameone.com](https://www.codenameone.com/) - Java/Kotlin geliştiricileri için açık kaynaklı, platformlar arası, mobil uygulama geliştirme araç zinciri. Sınırsız sayıda projeyle ticari kullanım için ücretsiz
  * [Daestro](https://daestro.com) - Bulut Sağlayıcıları ve Şirket İçi genelinde bilgi işlem işlerini çalıştırın. Ücretsiz katman, 10 adede kadar eşzamanlı iş çalıştırması, 2 bilgi işlem oluşturma, kendi kendine barındırılan bilgi işlem, 1 bulut sağlayıcı, 1 konteyner kayıt defteri ve 1 cron işi içerir.
  * [Deno Deploy](https://deno.com/deploy) - JavaScript, TypeScript ve WebAssembly'ı dünya çapında uçta çalıştıran dağıtılmış sistem. Ücretsiz katman, günde 100.000 isteği ve ayda 100 GiB veri aktarımını içerir.
  * [domcloud.co](https://domcloud.co) - GitHub, SSH ve MariaDB/Postgres veritabanıyla CI/CD sağlayan Linux barındırma hizmeti. Ücretsiz sürümde 1 GB depolama alanı ve 1 GB ağ/ay sınırı vardır ve ücretsiz alan adıyla sınırlıdır.
  * [encore.dev](https://encore.dev/) - Otomatik altyapı, ortak metinlerden bağımsız kod ve daha fazlasını sağlamak için statik analiz kullanan arka uç çerçevesi. Hobi projeleri için ücretsiz bulut barındırma içerir.
  * [flightcontrol.dev](https://flightcontrol.dev/) - Git push stili iş akışıyla web hizmetlerini, veritabanlarını ve daha fazlasını kendi AWS hesabınızda dağıtın. Kişisel GitHub depolarında 1 geliştiriciye sahip kullanıcılar için ücretsiz katman. AWS maliyetleri AWS aracılığıyla faturalandırılır ancak kredileri ve AWS ücretsiz kullanımını kullanabilirsiniz.
  * [gigalixir.com](https://gigalixir.com/) - Gigalixir, hiçbir zaman uyumayan ücretsiz bir örnek ve 2 bağlantı, 10.000 satırla sınırlı ve Elixir/Phoenix uygulamaları için yedek içermeyen ücretsiz katmanlı bir PostgreSQL veritabanı sağlar.
  * [leapcell](https://leapcell.io/) - Leapcell, hızlı büyümenizi sorunsuz bir şekilde desteklemek için ihtiyacınız olan her şeyi sağlayan güvenilir bir dağıtılmış uygulama platformudur. Ücretsiz planda 100 bin hizmet çağrısı, 10 bin eşzamansız görev ve 100 bin Redis komutu yer alıyor.
  * [Northflank](https://northflank.com) - Güçlü bir kullanıcı arayüzü, API ve CLI ile mikro hizmetler, işler ve yönetilen veritabanları oluşturun ve dağıtın. Sürüm kontrolünden ve harici Docker kayıtlarından kapsayıcıları sorunsuz bir şekilde ölçeklendirin. Ücretsiz katman iki hizmet, iki cron işi ve 1 veritabanı içerir.
  * [pipedream.com](https://pipedream.com) - Geliştiriciler için oluşturulmuş bir entegrasyon platformu. Herhangi bir tetikleyiciye dayalı olarak herhangi bir iş akışını geliştirin. İş akışları, [ücretsiz olarak](https://docs.pipedream.com/pricing/) çalıştırabileceğiniz kodlardır. Yönetilecek sunucu veya bulut kaynağı yok.
  * [Demiryolu](https://railway.app/) - Git tabanlı dağıtımlar, otomatik CI/CD ve yerleşik veritabanlarıyla her şeyi dağıtın. Ücretsiz katman her ay 5 ABD doları tutarında kredi içerir
  * [pythonanywhere.com](https://www.pythonanywhere.com/) - Bulut Python uygulaması barındırma. Başlangıç ​​hesabı ücretsizdir, kullanıcıadınız.pythonanywhere.com alan adınızda 1 Python web uygulaması, 512 MB özel dosya depolama alanı, bir MySQL veritabanı
  * [WunderGraph](https://cloud.wundergraph.com) - Modern API'leri hızla oluşturmanıza, göndermenize ve yönetmenize olanak tanıyan açık kaynaklı bir platform. Yerleşik CI/CD, GitHub entegrasyonu ve otomatik HTTPS. [Ücretsiz planda](https://wundergraph.com/pricing) en fazla 3 proje, 1 GB çıkış, ayda 300 dakika derleme süresi
  * [YepCode](https://yepcode.io) - API'leri ve hizmetleri sunucusuz bir ortamda bağlamak için hepsi bir arada platform. NoCode araçlarının tüm çevikliğini ve faydalarını, aynı zamanda programlama dillerini kullanmanın tüm gücüyle birlikte sunar. Ücretsiz katman, [1.000 evet](https://yepcode.io/pricing/) içerir.

**[⬆️Başa Dön](#table-of-contents)**

## BaaS

  * [Activepieces](https://www.activepieces.com) - Uygulamanızın arka ucunda birkaç uygulamayı birbirine bağlamak için otomasyon akışları oluşturun. Örneğin, uygulamanızda bir etkinlik tetiklendiğinde bir Slack mesajı gönderin veya bir Google E-Tablosu satırı ekleyin. Ayda 5.000'e kadar görevi ücretsiz yapın.
  * [back4app.com](https://www.back4app.com) - Back4App, Ayrıştırma Platformunu temel alan, kullanımı kolay, esnek ve ölçeklenebilir bir arka uçtur.
  * [backendless.com](https://backendless.com/) - Mobil ve Web Baas, ücretsiz 1 GB dosya depolama alanı, ayda 50.000 anlık bildirim ve tabloda 1000 veri nesnesi.
  * [bismuth.cloud](https://www.bismuth.cloud/) - Yapay zekamız, Python API'nizi işlev çalışma zamanımız ve barındırılan depolama alanımızda güçlendirecek, çevrimiçi düzenleyicimizde veya en sevdiğiniz araçlarla yerel olarak ücretsiz olarak oluşturacak ve barındıracaktır.
  * [Claw.cloud](https://run.claw.cloud) - 180 günden eski GitHub hesabına sahip kullanıcılara ayda 5 ABD doları tutarında ücretsiz kredi sunan bir PaaS platformu. Uygulamaları, veritabanlarını ve daha fazlasını barındırmak için mükemmeldir. ([Ücretsiz krediyle Kayıt Bağlantısı](https://ap-southeast-1.run.claw.cloud/signin)).
  * [connectycube.com](https://connectycube.com) - Sınırsız sohbet mesajları, p2p sesli ve görüntülü aramalar, dosya ekleri ve anında bildirimler. 1000 kullanıcıya kadar uygulamalar için ücretsiz.
  * [convex.dev](https://convex.dev/) - Hizmet olarak reaktif arka uç, verilerinizi (ilişkileri ve seri hale getirilebilir ACID işlemlerini içeren belgeler), sunucusuz işlevleri ve güncellemeleri çeşitli istemcilere yayınlamak için WebSocket'leri barındırır. Küçük projeler için ücretsiz - 1 milyona kadar kayıt, 5 milyona kadar aylık işlev çağrısı.
  * [ETLR](https://etlr.io) - YAML kullanarak otomasyon komut dosyalarını tanımlayın, sürümlendirin ve dağıtın. Sürükle ve bırak araçlarına geliştirici öncelikli bir alternatif. Zamanlanmış görevler, yapay zeka aracıları ve altyapı izleme için kullanılabilir. Ücretsiz katman ayda 100 kredi içerir.
  * [Flutter Flow](https://flutterflow.io) - Tek satır kod yazmadan Flutter Uygulamanızın kullanıcı arayüzünü oluşturun. Ayrıca Firebase entegrasyonu da var. Ücretsiz plan, UI Builder'a ve Ücretsiz şablonlara tam erişim içerir.
  * [getstream.io](https://getstream.io/) - Ölçeklenebilir Uygulama İçi Sohbet, Mesajlaşma, Video ve ses ile Akışları haftalar yerine birkaç saat içinde oluşturun
  * [IFTTT](https://ifttt.com) - Favori uygulamalarınızı ve cihazlarınızı otomatikleştirin. Ücretsiz 2 Applet
  * [Entegre olarak](https://integrately.com) - Sıkıcı görevleri tek tıklamayla otomatikleştirin. Ücretsiz 100 Görev, 15 Dakika
  * [LeanCloud](https://leancloud.app/) - Mobil arka uç. 1 GB veri depolama alanı, 256 MB bulut sunucusu, günde 3 bin API isteği ve günde 10 bin aktarma ücretsizdir. (API, Ayrıştırma Platformuna çok benzer)
  * [nhost.io](https://nhost.io) - Web ve mobil uygulamalar için sunucusuz arka uç. Ücretsiz plan PostgreSQL, GraphQL (Hasura), Kimlik Doğrulama, Depolama ve Sunucusuz İşlevleri içerir.
  * [onesignal.com](https://onesignal.com/) - Sınırsız ücretsiz anlık bildirimler. Sınırsız kişi ve Otomatik Isınma erişimiyle ayda 10.000 e-posta gönderimi.
  * [paraio.com](https://paraio.com) - Esnek kimlik doğrulama, tam metin arama ve önbelleğe alma özelliklerine sahip arka uç hizmeti API'si. Bir uygulama için ücretsiz, 1 GB uygulama verisi.
  * [pubnub.com](https://www.pubnub.com/) - Ayda 1 milyona kadar mesaj ve 100 aktif günlük cihaz için ücretsiz anlık bildirimler
  * [pushbots.com](https://pushbots.com/) - Anında bildirim hizmeti. Ayda 1,5 milyona kadar tıklama için ücretsiz
  * [pusher.com](https://pusher.com/beams) - 2000 aylık aktif kullanıcı için ücretsiz, sınırsız anlık bildirimler. iOS ve Android cihazlar için tek bir API.
  * [simperium.com](https://simperium.com/) - Verileri her yere anında ve otomatik olarak taşıyın, çoklu platform, yapılandırılmış verilerin sınırsız gönderimi ve depolanması, maks. 2.500 kullanıcı/ay
  * [Supabase](https://supabase.com) - Arka uçlar oluşturmak için Açık Kaynak Firebase Alternatifi. Ücretsiz Plan, Kimlik Doğrulama, Gerçek Zamanlı Veritabanı ve Nesne Depolama olanağı sunar.
  * [tyk.io](https://tyk.io/) - Kimlik doğrulama, kotalar, izleme ve analizle API yönetimi. Ücretsiz bulut teklifi
  * [zapier.com](https://zapier.com/) - Görevleri otomatikleştirmek için kullandığınız uygulamaları bağlayın. Her 15 dakikada bir beş zap ve ayda 100 görev
Güncelleme Zamanı, beş aktif otomasyon, web kancaları.


**[⬆️Başa Dön](#table-of-contents)**

## Low-code Platform

  * [appsmith](https://www.appsmith.com/) - Yönetici panelleri, dahili araçlar ve kontrol panelleri oluşturmaya yönelik az kodlu proje. 15'ten fazla veritabanı ve herhangi bir API ile entegre olur.
  * [BudiBase](https://budibase.com/) - Budibase, dakikalar içinde dahili uygulamalar oluşturmaya yönelik açık kaynaklı, az kodlu bir platformdur. PostgreSQL, MySQL, MSSQL, MongoDB, Rest API, Docker, K8s'i destekler
  * [Clappia](https://www.clappia.com) - Özelleştirilebilir mobil ve web uygulamalarıyla iş süreci uygulamaları oluşturmak için tasarlanmış az kodlu bir platform. Sürükle ve bırak arayüzü, Çevrimdışı Destek gibi özellikler, gerçek zamanlı konum izleme ve çeşitli üçüncü taraf hizmetlerle entegrasyon sunar
  * [lil'bots](https://www.lilbots.io/) - OpenAI, Anthropic, Firecrawl ve diğerleri gibi ücretsiz yerleşik API'leri kullanarak çevrimiçi komut dosyaları yazın ve çalıştırın. Yapay zeka aracıları/dahili araçlar oluşturmak ve ekiple paylaşmak için idealdir. Ücretsiz katman, API'lere tam erişim, AI kodlama asistanı ve ayda 10.000 yürütme kredisi içerir.
  * [manubes](https://www.manubes.com) - Endüstriyel üretim yönetimine odaklanan güçlü, kodsuz bulut platformu. Ayda 1 milyon iş akışı etkinliğine sahip bir kullanıcı için ücretsiz ([almanca olarak da mevcuttur](https://www.manubes.de)).
  * [Mendix](https://www.mendix.com/) - İşletmeler için Hızlı Uygulama Geliştirme, toplam kullanıcıları destekleyen sınırsız erişilebilir korumalı alan ortamları, uygulama başına 0,5 GB depolama ve 1 GB RAM. Ayrıca ücretsiz katmanda Studio ve Studio Pro IDE'lerine izin verilir.
  * [outsystems.com](https://www.outsystems.com/) - Şirket içi veya bulut için kurumsal web geliştirme PaaS, ücretsiz "kişisel ortam" teklifi, sınırsız koda ve 1 GB'a kadar veritabanına olanak tanır
  * [ReTool](https://retool.com/) - Dahili uygulamalar oluşturmaya yönelik düşük kodlu platform. Retool son derece hacklenebilir. JavaScript ve API ile yazabiliyorsanız Retool'da yapabilirsiniz. Ücretsiz katman ayda en fazla beş kullanıcıya, sınırsız uygulamaya ve API bağlantısına izin verir.
  * [ToolJet](https://www.tooljet.com/) - İş uygulamaları oluşturmak için genişletilebilir düşük kodlu çerçeve. Veritabanlarına, bulut depolama alanlarına, GraphQL'e, API uç noktalarına, Airtable'a vb. bağlanın ve sürükle ve bırak uygulama oluşturucuyu kullanarak uygulamalar oluşturun.
  * [UI Bakery](https://uibakery.io) - Özel web uygulamalarının daha hızlı oluşturulmasını sağlayan az kodlu platform. JavaScript, Python ve SQL aracılığıyla yüksek düzeyde özelleştirmeyle sürükle ve bırak yöntemini kullanarak kullanıcı arayüzü oluşturmayı destekler. Hem bulut hem de kendi kendine barındırılan çözümler olarak mevcuttur. 5 kullanıcıya kadar ücretsizdir.

**[⬆️Başa Dön](#table-of-contents)**

## Web Hosting

  * [Alwaysdata](https://www.alwaysdata.com/) - MySQL, PostgreSQL, RabbitMQ, .NET, Deno, Elixir, Go, Java, Lua, Node.js, PHP, Python, Ruby, Rust desteğiyle 1 GB ücretsiz web barındırma. Özel web sunucuları, FTP, WebDAV ve SSH üzerinden erişim. Posta kutusu, posta listesi ve uygulama yükleyicisi dahildir. Ücretsiz planda özel alan adı yok.
  * [Awardspace.com](https://www.awardspace.com) - Ücretsiz web barındırma + ücretsiz kısa alan adı, PHP, MySQL, Uygulama Yükleyici, E-posta Gönderme ve Reklamsız.
  * [Bubble](https://bubble.io/) - Bubble markasıyla ücretsiz, kodsuz web ve mobil uygulamalar oluşturmak için görsel programlama.
  * [dAppling Network](https://www.dappling.network/) - Çalışma süresini ve güvenliği artırmaya odaklanan ve kullanıcılar için ek bir erişim noktası sağlamaya odaklanan Web3 ön uçlarına yönelik merkezi olmayan web barındırma platformu.
  * [DigitalOcean](https://www.digitalocean.com/pricing) - Uygulama Platformu Başlangıç ​​katmanında ücretsiz olarak üç statik site oluşturun ve dağıtın.
  * [FreeFlarum](https://freeflarum.com/) - 250 kullanıcıya kadar topluluk destekli ücretsiz Flarum barındırma (filigranı alt bilgiden kaldırmak için bağış yapın).
  * [Kinsta Statik Site Barındırma](https://kinsta.com/static-site-hosting/) - SSL ile 100'e kadar statik siteyi, özel alan adlarını, 100 GB aylık bant genişliğini, 260'tan fazla Cloudflare CDN konumunu ücretsiz olarak dağıtın.
  * [MDB GO](https://mdbgo.com/) - İki haftalık Container TTL, proje başına 500 MB RAM, SFTP - 1G disk alanı ile bir proje için ücretsiz barındırma.
  * [Neocities](https://neocities.org) - Statik, 200 GB Bant Genişliğine sahip 1 GB ücretsiz depolama.
  * [Netlify](https://www.netlify.com/) - Aylık 300 kredi karşılığında ücretsiz olarak statik site/uygulama oluşturur, dağıtır ve barındırır (30 GB bant genişliğine eşittir).
  * [Oaysus](https://oaysus.com) - Geliştirici tarafından oluşturulmuş React, Vue veya Svelte bileşenleri için görsel sayfa oluşturucu. Ücretsiz katman, sınırsız sayfa, form gönderimi ve global CDN barındırma özelliğine sahip 1 siteyi içerir.
  * [PandaStack](https://www.pandastack.io/) - Geliştiricilere yönelik bir eko-sistem, farklı formatlarda web barındırma içerir (statik web barındırma, kapsayıcı tabanlı web barındırma, wordpress ve birkaç tıklamayla erişilebilen diğer birçok yönetilen uygulama). Bir ücretsiz web barındırma (statik veya konteynerli) ve 100 GB Bant Genişliği ve 300 Dakika/ay ile bir ücretsiz veritabanı.
  * [pantheon.io](https://pantheon.io/) - Drupal ve WordPress barındırma, otomatik DevOps ve ölçeklenebilir altyapı. Geliştiriciler ve ajanslar için ücretsiz. Özel alan adı yok.
  * [Qoddi](https://qoddi.com) - Geliştirici merkezli bir yaklaşıma ve her şey dahil özelliklere sahip Heroku'ya benzer PaaS hizmeti. Statik varlıklar, hazırlama ve geliştirici uygulamaları için ücretsiz katman.
  * [readthedocs.org](https://readthedocs.org/) - Sürüm oluşturma, PDF oluşturma ve daha fazlasıyla ücretsiz belge barındırma
  * [render.com](https://render.com) - Ücretsiz SSL, küresel bir CDN, özel ağlar, Git'ten otomatik dağıtımlar ve web hizmetleri, veritabanları ve statik web sayfaları için tamamen ücretsiz planlar içeren uygulamalar ve siteler oluşturmak ve çalıştırmak için birleştirilmiş bulut.
  * [Serv00.com](https://serv00.com/) - Günlük yedeklemelerle (7 gün) 3 GB ücretsiz web barındırma. Destek: Crontab işleri, SSH erişimi, depolar (GIT, SVN ve Mercurial), destek: MySQL, PostgreSQL, MongoDB, PHP, Node.js, Python, Ruby, Java, Perl, TCL/TK, Lua, Erlang, Rust, Pascal, C, C++, D, R ve çok daha fazlası.
  * [SourceForge](https://sourceforge.net/) - Açık Kaynak yazılımını ücretsiz bulun, oluşturun ve yayınlayın
  * [surge.sh](https://surge.sh/) - Ön Uç geliştiriciler için statik web yayınlama. Özel alan adı desteğiyle sınırsız site
  * [tilda.cc](https://tilda.cc/) - Bir site, 50 sayfa, 50 MB depolama, 170'den fazla mevcut blok arasında yalnızca önceden tanımlanmış ana bloklar, yazı tipi yok, site simgesi yok ve özel alan adı yok
  * [Vercel](https://vercel.com/) - Her "git push" işleminizde ücretsiz SSL, global CDN ve benzersiz Önizleme URL'leri ile web uygulamaları oluşturun, dağıtın ve barındırın. Next.js ve diğer Statik Site Oluşturucular için mükemmeldir.
  * [Versoly](https://versoly.com/) - SaaS odaklı web sitesi oluşturucu - sınırsız web sitesi, 70'ten fazla blok, beş şablon, özel CSS, favicon, SEO ve formlar. Özel alan adı yok.

**[⬆️Başa Dön](#table-of-contents)**

## DNS

  * [1.1.1.1](https://developers.cloudflare.com/1.1.1.1/) - Cloudflare tarafından sağlanan hızlı ve güvenli (DNS sorgunuzu şifreleyin) ücretsiz genel DNS Çözümleyici. İnternet sağlayıcınızın DNS engellemesini aşmak, DNS sorgu casusluğunu önlemek ve [yetişkinlere yönelik ve kötü amaçlı yazılım içeriğini engellemek için](https://developers.cloudflare.com/1.1.1.1/1.1.1.1-for-families) kullanışlıdır. Ayrıca [API aracılığıyla](https://developers.cloudflare.com/1.1.1.1/encrypted-dns/dns-over-https/make-api-requests) da kullanılabilir. Not: Yalnızca bir DNS çözümleyicidir, DNS barındırıcısı değildir.
  * [1984.is](https://www.1984.is/product/freedns/) - API ve diğer birçok ücretsiz DNS özelliği içeren ücretsiz DNS hizmeti.
  * [cloudns.net](https://www.cloudns.net/) - 50 kayıtla 1 alana kadar ücretsiz DNS barındırma
  * [deSEC](https://desec.io) - Güvenlik göz önünde bulundurularak tasarlanmış, API destekli ücretsiz DNS barındırma. Açık kaynaklı yazılım üzerinde çalışır ve [SSE](https://www.securesystems.de/) tarafından desteklenir.
  * [dns.he.net](https://dns.he.net/) - Dinamik DNS Desteği ile ücretsiz DNS barındırma hizmeti
  * [dnspod.com](https://www.dnspod.com/) - Ücretsiz DNS barındırma.
  * [duckdns.org](https://www.duckdns.org/) - Ücretsiz katmanda en fazla 5 alan adı içeren ücretsiz DDNS. Çeşitli kurulumlar için yapılandırma kılavuzları ile.
  * [Dynv6.com](https://dynv6.com/) - [API desteği](https://dynv6.com/docs/apis) ve birçok dns kayıt türünün (CNAME, MX, SPF, SRV, TXT ve diğerleri gibi) yönetimi ile ücretsiz DDNS hizmeti.
  * [freedns.afraid.org](https://freedns.afraid.org/) - Ücretsiz DNS barındırma. Ayrıca, çok sayıda genel kullanıcıya [katkıda bulunulan alan adlarına](https://freedns.afraid.org/domain/registry/) dayalı olarak ücretsiz alt alan adları sağlayın. Kaydolduktan sonra "Alt Alan Adları" menüsünden ücretsiz alt alan adları alın.
  * [Glauca](https://docs.glauca.digital/hexdns/) - 3 alana kadar ücretsiz DNS barındırma ve DNSSEC desteği
  * [Hetzner](https://www.hetzner.com/dns-console) - Hetzner'den API desteğiyle ücretsiz DNS barındırma.
  * [huaweicloud.com](https://www.huaweicloud.com/intl/en-us/product/dns.html) - Huawei tarafından ücretsiz DNS barındırma
  * [LocalCert](https://localcert.net) - Özel ağlarda kullanım için genel CA'larla uyumlu ücretsiz `.localcert.net` alt alanları
  * [luadns.com](https://www.luadns.com/) - Ücretsiz DNS barındırma, üç alan adı, makul sınırlarla tüm özellikler
  * [namecheap.com](https://www.namecheap.com/domains/freedns/) - Ücretsiz DNS. Alan adı sayısında sınırlama yok
  * [nextdns.io](https://nextdns.io) - DNS tabanlı güvenlik duvarı, aylık 300.000 ücretsiz sorgu
  * [noip.at](https://noip.at/) - Kayıt, takip, kayıt veya reklam gerektirmeden ücretsiz DDNS hizmeti. Alan adlarında sınır yok.
  * [noip](https://www.noip.com/) - her 30 günde bir onay ile en fazla 3 ana bilgisayar adına ücretsiz izin veren dinamik bir DNS hizmeti
  * [sslip.io](https://sslip.io/) - Katıştırılmış IP adresine sahip bir ana bilgisayar adı ile sorgulandığında bu IP adresini döndüren ücretsiz DNS hizmeti.
  * [VolaryDDNS](https://volaryddns.net) - Abonelik veya reklam içermeyen, ücretsiz, yüksek performanslı DDNS
  * [zilore.com](https://zilore.com/en/dns) - 5 alan adı için ücretsiz DNS barındırma.
  * [zoneedit.com](https://www.zoneedit.com/free-dns/) - Dinamik DNS Desteği ile ücretsiz DNS barındırma.
  * [Zonomi](https://zonomi.com/) - Anında DNS yayılımıyla ücretsiz DNS barındırma hizmeti. Ücretsiz plan: 10 DNS kaydına kadar 1 DNS bölgesi (alan adı).

**[⬆️Başa Dön](#table-of-contents)**

## Domain

  * [DigitalPlat](https://domain.digitalplat.org) - Ücretsiz alt alan adları.
  * [isroot.in](https://isroot.in) - Ücretsiz isroot.in alt alan adları.
  * [pp.ua](https://nic.ua/) - Ücretsiz pp.ua alt alan adları.

**[⬆️Başa Dön](#table-of-contents)**

## IaaS

  * [4EVERLAND](https://www.4everland.org/) - AWS S3 ile uyumludur - API'ler, arayüz işlemleri, CLI ve diğer yükleme yöntemleri, IPFS ve Arweave ağlarından dosyaları güvenli, kullanışlı ve verimli bir şekilde yükleyin ve saklayın. Kayıtlı kullanıcılar 6 GB IPFS depolama alanına ve 300 MB Arweave depolama alanına ücretsiz olarak sahip olabilir. 150 KB'tan küçük tüm Arweave dosyası yüklemeleri ücretsizdir.
  * [backblaze.com](https://www.backblaze.com/b2/) - Backblaze B2 bulut depolama alanı. Sınırsız süre boyunca ücretsiz 10 GB (Amazon S3 benzeri) nesne depolama alanı
  * [C2 Nesne Depolama](https://c2.synology.com/en-us/pricing/object-storage) - S3 uyumlu nesne depolama. 15 GB ücretsiz depolama alanı ve ayda 15 GB indirme.
  * [filebase.com](https://filebase.com/) - Blockchain Tarafından Desteklenen S3 Uyumlu Nesne Depolama. Sınırsız bir süre için 5 GB ücretsiz depolama alanı.

**[⬆️Başa Dön](#table-of-contents)**

## Managed Data Services

  * [8base.com](https://www.8base.com/) - 8base, MySQL ve GraphQL ve sunucusuz hizmet olarak arka uç üzerine inşa edilmiş JavaScript geliştiricileri için oluşturulmuş tam yığın, düşük kodlu bir geliştirme platformudur. Bir kullanıcı arayüzü uygulama oluşturucu kullanarak hızlı bir şekilde web uygulamaları oluşturmaya başlamanıza ve hızlı bir şekilde ölçeklendirmenize olanak tanır. Ücretsiz katmanda satırlar bulunur: 2.500, Depolama: 500, Sunucusuz bilgi işlem: 1 Gb/saat ve istemci uygulaması kullanıcıları: 5.
  * [airtable.com](https://airtable.com/) - Bir e-tabloya benziyor ancak sınırsız tabana, 1.200 satır/tabana ve ayda 1.000 API isteğine sahip ilişkisel bir veritabanıdır
  * [Aiven](https://aiven.io/) - Aiven, açık kaynaklı veri platformunda ücretsiz PostgreSQL, MySQL ve Valkey (Redis uyumlu) planları sunar. Tek düğüm, 1 CPU, 1 GB RAM ve PostgreSQL ve MySQL için 1 GB depolama. Daha kapsamlı planlara veya bulutlar arasında kolay geçiş.
  * [CockroachDB Cloud](https://www.cockroachlabs.com/pricing/) - Ücretsiz katman, ayda 50 milyon RU ve 10 GiB depolama (15$ değerinde) ücretsiz sunar. ([İstek Birimleri Nedir](https://www.cockroachlabs.com/docs/cockroachcloud/metrics-request-units.html))
  * [codehooks.io](https://codehooks.io/) - İşlevler, Mongdb benzeri sorgular, anahtar/değer aramaları, iş sistemi, gerçek zamanlı mesajlar, çalışan kuyrukları, güçlü bir CLI ve web tabanlı veri yöneticisi ile kullanımı kolay JavaScript sunucusuz API/arka uç ve NoSQL veritabanı hizmeti. Ücretsiz planda 5 GB depolama alanı ve dakikada 60/API araması bulunur. 2 geliştirici dahil. Kredi kartına gerek yok.
  * [Couchbase Capella](https://www.couchbase.com/products/capella/) - geliştiricilerin IoT'den yapay zekaya kadar yeni nesil uygulamalar oluşturması için tasarlanmış, 1 düğüm ve 8 GB depolama alanına sahip, sonsuza kadar ücretsiz katmanlı, tam olarak yönetilen bir veritabanı kümesi dağıtın
  * [CrateDB](https://crate.io/) - Gerçek zamanlı analiz için dağıtılmış Açık Kaynak SQL veritabanı. [Ücretsiz Kullanım CRFREE](https://crate.io/lp-crfree): 2 CPU, 2 GiB bellek, 8 GiB depolama alanına sahip tek düğüm. Kuruluş başına bir küme; ödeme yöntemi gerekmez.
  * [filess.io](https://filess.io) - filess.io, ücretsiz olarak aşağıdaki DBMS'lerin veritabanı başına 10 MB'a kadar iki veritabanı oluşturabileceğiniz bir platformdur: MySQL, MariaDB, MongoDB ve PostgreSQL.
  * [InfluxDB](https://www.influxdata.com/) - Timeseries veritabanı, 3 MB/5 dakikaya kadar ücretsiz yazma, 30 MB/5 dakikaya kadar okuma ve 10.000 kardinalite serisi
  * [MemCachier](https://www.memcachier.com/) - Yönetilen Memcache hizmeti. 25 MB'a kadar ücretsiz, 1 Proxy Sunucu ve temel analizler
  * [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) - ücretsiz katman 512 MB verir
  * [Neo4j Aura](https://neo4j.com/cloud/aura/) - Cypher sorgu dili ve REST API ile yönetilen yerel Graph DBMS/analiz platformu. Grafik boyutunda sınırlamalar (50 bin düğüm, 175 bin ilişki).
  * [Neon](https://neon.tech/) - Yönetilen PostgreSQL, 0,5 GB depolama (toplam), 1 Proje, 10 şube, Sınırsız Veritabanları, her zaman kullanılabilir birincil şube (5 dakika sonra otomatik askıya alma), birincil olmayan şube hesaplaması için ayda 20 saat Aktif süre (toplam).
  * [Nile](https://www.thenile.dev/) - B2B uygulamaları için bir Postgres platformu. Sınırsız veritabanları, Kapatma olmadan her zaman kullanılabilir, 1 GB depolama (toplam), 50 milyon sorgu belirteci, otomatik ölçeklendirme, sınırsız vektör yerleştirme
  * [Prisma Postgres](https://prisma.io/postgres) - Süper hızlı barındırılan Postgres, tek çekirdekler üzerine kuruludur ve yalın donanım üzerinde çalışır, 1 GB depolama, 10 veritabanı, Prisma ORM ile entegredir.
  * [restdb.io](https://restdb.io/) - hızlı ve basit bir NoSQL bulut veritabanı hizmeti. Restdb.io ile şema, ilişkiler, otomatik REST API (MongoDB benzeri sorgularla) ve verilerle çalışmak için verimli, çok kullanıcılı bir yönetici kullanıcı arayüzüne sahip olursunuz. Ücretsiz plan 3 kullanıcıya, 2500 kayda ve saniyede 1 API isteğine izin verir.
  * [scalingo.com](https://scalingo.com/) - Öncelikle bir PaaS ancak 128 MB ila 192 MB ücretsiz MySQL, PostgreSQL veya MongoDB katmanı sunuyor
  * [SeaTable](https://seatable.io/) - Seafile ekibi tarafından oluşturulan esnek, Elektronik Tablo benzeri Veritabanı. sınırsız tablo, 2.000 satır, 1 aylık versiyonlama, 25'e kadar ekip üyesi.
  * [skyvia.com](https://skyvia.com/) - Bulut Veri Platformu ücretsiz bir katman sunar ve beta sürümde tüm planlar tamamen ücretsizdir
  * [StackBy](https://stackby.com/) - Elektronik tabloların esnekliğini, veritabanlarının gücünü ve favori iş uygulamalarınızla yerleşik entegrasyonları birleştiren tek araç. Ücretsiz plan sınırsız kullanıcı, on yığın ve yığın başına 2 GB ek içerir.
  * [Tinybird](https://tinybird.co) - HTTP üzerinden bağlantısız veri alımına sahip, sunucusuz yönetilen bir ClickHouse ve SQL sorgularını yönetilen HTTP API'leri olarak yayınlamanıza olanak tanır. Ücretsiz katmanda, 10 GB depolama + günlük 1000 API isteğinde zaman sınırı yoktur.
  * [Turso by ChiselStrike](https://chiselstrike.com/) - Turso, Uç Veritabanındaki SQLite Geliştirici Deneyimidir. Turso, Free Forever başlangıç ​​planı, 9 GB toplam depolama, 500'e kadar veritabanı, 3'e kadar konum, ayda 1 milyar satır okuma ve SQLite ile Yerel geliştirme desteği sağlar.
  * [Upstash](https://upstash.com/) - Aylık 500 bine kadar komut, 256 MB maksimum veritabanı boyutu ve 20 eşzamanlı bağlantıya kadar ücretsiz kullanıma sahip Sunucusuz Redis
  * [Xata Lite](https://lite.xata.io/) - Xata Lite, yerleşik güçlü arama ve analiz özelliklerine sahip sunucusuz bir veritabanıdır. Tek bir API, birden çok tür uyumlu istemci kitaplığı ve geliştirme iş akışınız için optimize edilmiş. Ücretsiz plan, duraklama veya soğuk başlatma olmadan 10 şube ve 15 GB depolama alanı sağlar.

**[⬆️Başa Dön](#table-of-contents)**

## Tunneling, WebRTC, Web Socket Servers and Other Routers

  * [btunnel](https://www.btunnel.in/) - Localhost'u ve yerel TCP sunucusunu internete açık hale getirir. Ücretsiz plan, dosya sunucusunu, özel http isteği ve yanıt başlıklarını, temel kimlik doğrulama korumasını ve 1 saatlik tünel zaman aşımını içerir.
  * [cname.dev](https://cname.dev/) - Ücretsiz ve güvenli dinamik ters proxy hizmeti.
  * [conveyor.cloud](https://conveyor.cloud/) - IIS Express'i yerel ağa veya bir tünel üzerinden genel bir URL'ye kullanıma sunmaya yönelik Visual Studio uzantısı.
  * [Expose](https://expose.dev/) - Yerel siteleri güvenli tüneller aracılığıyla açığa çıkarın. Ücretsiz plan bir AB Sunucusu, Rastgele alt alanlar ve Tek kullanıcılar içerir.
  * [Hamachi](https://www.vpn.net/) - LogMeIn Hamachi, 5 kişiye kadar sınırsız ağlara izin veren ücretsiz bir planla LAN benzeri ağları dağıtılmış ekiplere güvenli bir şekilde genişletmenize olanak tanıyan, barındırılan bir VPN hizmetidir
  * [Hookdeck](https://hookdeck.com/pricing) - Web kancalarınızı her yerden geliştirin, test edin ve izleyin. Üç günlük saklama süresiyle ayda 100.000 istek ve 100.000 deneme.
  * [localhost.run](https://localhost.run/) - Yerel olarak çalışan sunucuları bir tünel üzerinden genel bir URL'ye gösterin.
  * [localtunnel](https://theboroer.github.io/localtunnel-www/) - Yerel olarak çalışan sunucuları bir tünel üzerinden genel bir URL'ye gösterin. Ücretsiz barındırılan sürüm ve [açık kaynak](https://github.com/localtunnel/localtunnel).
  * [LocalXpose](https://localxpose.io) - Localhost sunucularınızı internete açmanıza olanak tanıyan ters proxy. Ücretsiz planın tünel ömrü 15 dakikadır.
  * [ngrok.com](https://ngrok.com/) - Yerel olarak çalışan sunucuları bir tünel üzerinden genel bir URL'ye gösterin.
  * [Pinggy](https://pinggy.io) - Tek komutla localhost için genel URL'ler, indirme gerekmez. HTTPS / TCP / TLS tünelleri. Ücretsiz planın tünel ömrü 60 dakikadır.
  * [Radmin VPN](https://www.radmin-vpn.com/) - VPN'yi etkinleştiren LAN benzeri bir ağ aracılığıyla birden fazla bilgisayarı birbirine bağlayın. Sınırsız akran. (Hamachi alternatifi)
  * [serveo](https://serveo.net/) - Yerel sunucuları internete açın. Kurulum yok, kayıt yok. Ücretsiz alt alan adı, sınır yok.
  * [stun:global.stun.twilio.com:3478?transport=udp](stun:global.stun.twilio.com:3478?transport=udp) - Twilio STUN
  * [stun:stun.l.google.com:19302](stun:stun.l.google.com:19302) - Google STUN
  * [Tailscale](https://tailscale.com/) - Açık kaynaklı WireGuard protokolünü kullanan sıfır yapılandırmalı VPN. MacOS, iOS, Windows, Linux ve Android cihazlara yüklenir. 100 cihaz ve üç kullanıcıyla kişisel kullanıma yönelik ücretsiz plan.
  * [webhookrelay.com](https://webhookrelay.com) - Tüm web kancalarınızı genel veya dahili (ör. localhost) hedeflere yönetin, hata ayıklayın, dağıtın ve proxy yapın. Ayrıca, genel bir HTTP uç noktası (`https://yoursubdomain.webrelay.io <----> http://localhost:8080`).) alarak özel bir ağda çalışan sunucuları bir tünel üzerinden açığa çıkarın.
  * [Xirsys](https://www.xirsys.com/pricing/) - Sınırsız STUN kullanımı + 500 MB aylık TURN bant genişliği, sınırlı bant genişliği, tek coğrafi bölge.
  * [ZeroTier](https://www.zerotier.com) - FOSS, hizmet olarak sanal Ethernet'i yönetti. Ücretsiz planda 25 istemciden oluşan sınırsız uçtan uca şifrelenmiş ağ. Masaüstü/mobil/NA için istemciler; özel yönlendirme kurallarının yapılandırılması ve özel ağlardaki yeni istemci düğümlerinin onaylanması için web arayüzü

**[⬆️Başa Dön](#table-of-contents)**

## Issue Tracking and Project Management

  * [acunote.com](https://www.acunote.com/) - En fazla 5 ekip üyesi için ücretsiz proje yönetimi ve SCRUM yazılımı
  * [asana.com](https://asana.com/) - Ortak çalışanlarla özel proje için ücretsiz
  * [Backlog](https://backlog.com) - Ekibinizin harika projeler yayınlamak için ihtiyaç duyduğu her şey tek bir platformda. Ücretsiz plan, on kullanıcılı ve 100 MB depolama alanına sahip 1 Proje sunar.
  * [Basecamp](https://basecamp.com/personal) - Yapılacaklar listeleri, kilometre taşı yönetimi, forum benzeri mesajlaşma, dosya paylaşımı ve zaman takibi. En fazla 3 proje, 20 kullanıcı ve 1 GB depolama alanı.
  * [bitrix24.com](https://www.bitrix24.com/) - İntranet ve proje yönetimi aracı. Ücretsiz planın sınırsız kullanıcı için 5GB'ı vardır.
  * [cacoo.com](https://cacoo.com/) - Çevrimiçi gerçek zamanlı diyagramlar: akış şeması, UML, ağ. Ücretsiz maks. 15 kullanıcı/diyagram, 25 sayfa
  * [clickup.com](https://clickup.com/) - Proje yönetimi. Bulut depolama alanına sahip ücretsiz, premium sürüm. Mobil uygulamalar ve Git entegrasyonları mevcuttur.
  * [Clockify](https://clockify.me) - Projeler genelinde çalışma saatlerini izlemenizi sağlayan zaman izleyici ve zaman çizelgesi uygulaması. Sınırsız kullanıcı, sonsuza kadar ücretsiz.
  * [Cloudcraft](https://cloudcraft.co/) - Cloudcraft görsel tasarımcısıyla dakikalar içinde, canlı verileri de gösteren akıllı bileşenlerle AWS için optimize edilmiş profesyonel bir mimari diyagramı tasarlayın. Ücretsiz planın tek kullanıcı için sınırsız özel diyagramları vardır.
  * [Confluence](https://www.atlassian.com/software/confluence) - Atlassian'ın içerik işbirliği aracı, ekiplerin verimli bir şekilde işbirliği yapmasına ve bilgiyi paylaşmasına yardımcı olmak için kullanılır. 10 kullanıcıya kadar ücretsiz plan.
  * [Crosswork](https://crosswork.app/) - Çok yönlü proje yönetimi platformu. 3 projeye kadar ücretsiz, sınırsız kullanıcı, 1 GB depolama alanı.
  * [diagrams.net](https://app.diagrams.net/) - Google Drive, OneDrive veya Dropbox'ta yerel olarak depolanan çevrimiçi diyagramlar. Tüm özellikler ve depolama seviyeleri için ücretsiz
  * [easyretro.io](https://www.easyretro.io/) - Basit ve sezgisel sprint retrospektif aracı. Ücretsiz planda üç halka açık pano ve pano başına ayda bir anket bulunur.
  * [freedcamp.com](https://freedcamp.com/) - görevler, tartışmalar, kilometre taşları, zaman takibi, takvim, dosyalar ve şifre yöneticisi. Sınırsız proje, kullanıcı ve dosya depolama alanıyla ücretsiz plan.
  * [GForge](https://gforge.com) - Kendi kendine tesis ve SaaS seçenekleriyle karmaşık projeler için Proje Yönetimi ve Sorun İzleme araç seti. SaaS ücretsiz planı, ilk beş kullanıcıya Açık Kaynak Projeleri için ücretsiz ve ücretsiz teklif sunar.
  * [gleek.io](https://www.gleek.io) - Geliştiriciler için ücretsiz açıklama-diyagram aracı. Anahtar kelimenizi kullanarak resmi olmayan UML sınıfı, nesne veya varlık-ilişki diyagramları oluşturun.
  * [GraphQL Inspector](https://github.com/marketplace/graphql-inspector) - GraphQL Inspector, iki GraphQL şeması arasındaki değişikliklerin bir listesini çıkarır. Her farklılık tam olarak açıklanmış ve kırılmaz, kırılmaz veya tehlikeli olarak işaretlenmiştir.
  * [Helploom](https://helploom.com) - Sonsuza kadar ücretsiz planda canlı sohbet sunan müşteri destek yazılımı. Basit, hafif ve güzel. Kurulum basit bir kopyala-yapıştır komut dosyasıdır. Bir geliştirici tarafından oluşturuldu.
  * [Hygger](https://hygger.io) - Proje yönetimi platformu. Ücretsiz plan, 100 MB Depolama alanına sahip sınırsız kullanıcı, proje ve pano sunar.
  * [Ilograph](https://www.ilograph.com/) - kullanıcıların altyapılarını çeşitli perspektiflerden ve ayrıntı düzeylerinden görmelerine olanak tanıyan etkileşimli diyagramlar. Grafikler kodla ifade edilebilir. Ücretsiz katmanda 3 izleyiciye kadar sınırsız özel diyagram bulunur.
  * [Jira](https://www.atlassian.com/software/jira) - Birçok kurumsal ortamda kullanılan gelişmiş yazılım geliştirme proje yönetimi aracı. 10 kullanıcıya kadar ücretsiz plan.
  * [kan.bn](https://kan.bn/) - İşinizi organize etmenize, ilerlemeyi takip etmenize ve sonuçları tek bir yerde sunmanıza yardımcı olan güçlü, esnek bir kanban uygulaması. Sınırsız pano, sınırsız liste, sınırsız kart için 1 kullanıcıya kadar ücretsiz plan.
  * [kanbanflow.com](https://kanbanflow.com/) - Yönetim kurulu tabanlı proje yönetimi. Daha fazla seçeneğe sahip ücretsiz, premium sürüm
  * [kanbantool.com](https://kanbantool.com/) - Kanban panosuna dayalı proje yönetimi. Ücretsiz planda ek veya dosya olmayan iki pano ve iki kullanıcı bulunur.
  * [Kitemaker.co](https://kitemaker.co) - Ürün geliştirme sürecinin tüm aşamalarında işbirliği yapın ve Slack, Discord, Figma ve Github'daki çalışmaları takip edin. Sınırsız kullanıcı, sınırsız alan. 250 iş öğesine kadar ücretsiz plan.
  * [Kiter.app](https://www.kiter.app/) - Herkesin iş aramasını organize etmesine ve görüşmeleri, fırsatları ve bağlantıları izlemesine izin verin. Güçlü web uygulaması ve Chrome uzantısı. Tamamen ücretsiz.
  * [Kumu.io](https://kumu.io/) - Animasyon, dekorasyon, filtreler, kümeleme, e-tablo içe aktarma vb. içeren ilişki haritaları. Ücretsiz katman, sınırsız kamu projelerine izin verir. Grafik boyutu sınırsız. Öğrenciler için ücretsiz özel projeler. Dosyanızı herkese açık olarak çevrimiçi bırakmamayı (yükleme, düzenleme, indirme, atma) tercih etmiyorsanız, korumalı alan modu kullanılabilir.
  * [leiga.com](https://www.leiga.com/) - Leiga, projelerinizi otomatik olarak yönetmek için yapay zekayı kullanan, ekibinizin odaklanmış kalmasına ve muazzam potansiyeli ortaya çıkarmasına yardımcı olarak projelerinizin planlandığı gibi ilerlemesini sağlayan bir SaaS ürünüdür. 10 kullanıcıya kadar ücretsiz, 20 özel alan, 2 GB depolama alanı, AI ile Video Kaydı video başına 5 dakika ile sınırlıdır, Otomasyon kullanıcı başına ayda 20 dakikayla çalışır.
  * [Doğrusal](https://linear.app/) - Kolaylaştırılmış bir arayüze sahip sorun izleyici. Sınırsız üyeye ücretsiz, 10 MB'a kadar dosya yükleme boyutu, 250 sayı (Arşiv hariç)
  * [Lucidchart](https://www.lucidchart.com/) - İşbirliği özelliklerine sahip çevrimiçi bir diyagram aracı. Düzenlenebilir üç belge, 100 profesyonel şablon ve temel işbirliği özellikleri içeren ücretsiz plan.
  * [MeisterTask](https://www.meistertask.com/) - Ekipler için çevrimiçi görev yönetimi. 3 projeye kadar ücretsiz ve sınırsız proje üyesi.
  * [MeuScrum](https://www.meuscrum.com/en) - Kanban panosuyla ücretsiz çevrimiçi saldırı aracı
  * [nTask](https://www.ntaskmanager.com/) - Ekiplerinizin işbirliği yapmasına, planlama yapmasına, analiz etmesine ve günlük görevleri yönetmesine olanak tanıyan proje yönetimi yazılımı. Temel plan, 100 MB depolama alanı ve beş kullanıcı/ekip ile sonsuza kadar ücretsizdir. Sınırsız çalışma alanı, toplantılar, ödevler, zaman çizelgeleri ve sorun takibi.
  * [Plane](https://plane.so/) - Plane basit, genişletilebilir, açık kaynaklı bir proje ve ürün yönetimi aracıdır. Sınırsız üyeye ücretsiz, 5 MB'a kadar dosya yükleme boyutu, 1000 sayı.
  * [planitpoker.com](https://www.planitpoker.com/) - Ücretsiz çevrimiçi planlama pokeri (tahmin aracı)
  * [point.poker](https://www.point.poker/) - Çevrimiçi Planlama Pokeri (fikir birliğine dayalı tahmin aracı). Sınırsız kullanıcı, ekip, oturum, tur ve oylama için ücretsiz. Kayıt olmanıza gerek yok.
  * [Pulse.red](https://pulse.red) - Projeler için ücretsiz Minimalist Zaman Takipçisi ve Zaman Çizelgesi uygulaması.
  * [ScrumFast](https://www.scrumfast.com) - Çok sezgisel bir arayüze sahip Scrum panosu, 5 kullanıcıya kadar ücretsiz.
  * [Sflow](https://sflow.io) - sflow.io, özellikle dış kaynak kullanımı ve kuruluşlar arası işbirliği projeleri için çevik yazılım geliştirme, pazarlama, satış ve müşteri desteği için oluşturulmuş bir proje yönetimi aracıdır. 3 projeye ve beş üyeye kadar ücretsiz plan.
  * [Shake](https://www.shakebugs.com/) - Mobil uygulamalar için uygulama içi hata raporlama ve geri bildirim aracı. Ücretsiz plan, uygulama/ay başına on hata raporu.
  * [Kısayol](https://shortcut.com/) - Proje yönetimi platformu. 10 kullanıcıya kadar sonsuza kadar ücretsiz.
  * [taiga.io](https://taiga.io/) - Yeni başlayanlar ve çevik geliştiriciler için proje yönetimi platformu, Açık Kaynak için ücretsiz
  * [taskade.com](https://www.taskade.com/) - Gerçek zamanlı ortak çalışmaya dayalı görev listeleri ve ekip taslakları. Ücretsiz planda sınırsız görev ve proje içeren bir çalışma alanı bulunur; 1 GB dosya depolama alanı; 1 haftalık proje geçmişi; ve video toplantısı başına beş katılımcı.
  * [Teaminal](https://www.teaminal.com) - Uzaktaki ekipler için ayakta durma, retro ve sprint planlama aracı. 15 kullanıcıya kadar ücretsizdir.
  * [teamwork.com](https://teamwork.com/) - Proje yönetimi ve Ekip Sohbeti. Beş kullanıcı ve iki proje için ücretsiz. Premium planlar mevcuttur.
  * [teleretro.com](https://www.teleretro.com/) - Buz kırıcılar, gifler ve emojiler içeren basit ve eğlenceli geçmişe dönük araç. Ücretsiz plan üç retro ve sınırsız üye içerir.
  * [Tenzu](https://tenzu.net/) - Çevik ekipler için hafif proje yönetimi aracı. SaaS ücretsiz katkılara dayanır; kullanıcılar her zaman 0 vermeyi seçebilir ve herhangi bir ödeme duvarı özelliği yoktur {[more information](https://tenzu.net/pricing/)}
  * [titanapps.io](https://titanapps.io/) - Jira ve monday.com için sorunlar/görevler içinde yapılandırılmış kontrol listeleri, şablonlar ve onaylar sunan üretkenlik araçları. Küçük ekipler için ücretsiz plan mevcuttur.
  * [todoist.com](https://todoist.com/) - İşbirliğine dayalı ve bireysel görev yönetimi. Ücretsiz plan şunları içerir: 5 aktif proje, projede beş kullanıcı, 5 MB'a kadar dosya yükleme, üç filtre ve bir haftalık etkinlik geçmişi.
  * [Toggl](https://toggl.com/) - İki ücretsiz üretkenlik aracı sağlar. Ücretsiz bir planla zaman yönetimi ve takip uygulaması için [Toggl Track](https://toggl.com/track/), serbest çalışanlar düşünülerek tasarlanmış kesintisiz zaman takibi ve raporlama sağlar. Sınırsız izleme kaydına, projeye, müşteriye, etikete, raporlamaya ve daha fazlasına sahiptir. Ve sınırsız görev, kilometre taşı ve zaman çizelgesine sahip, yalnız geliştiricilere yönelik ücretsiz bir planla görev planlaması için [Toggl Plan](https://toggl.com/plan/).
  * [trello.com](https://trello.com/) - Yönetim kurulu tabanlı proje yönetimi. Sınırsız Kişisel Pano, 10 Takım Panosu.
  * [Tweek](https://tweek.so/) - Basit Haftalık Yapılacaklar Takvimi ve Görev Yönetimi.
  * [Wikifactory](https://wikifactory.com/) - Projeler, VCS ve Sorunlarla Ürün Tasarımı Hizmeti. Ücretsiz plan sınırsız proje ve ortak çalışan ile 3 GB depolama alanı sunar.
  * [Yodiz](https://www.yodiz.com/) - Çevik geliştirme ve sorun takibi. 3 kullanıcıya kadar ücretsiz, sınırsız proje.
  * [YouTrack](https://www.jetbrains.com/youtrack/buy/#edition=incloud) - FOSS projeleri ve özel projeler için ücretsiz olarak barındırılan YouTrack (InCloud) (üç kullanıcı için ücretsiz). Zaman takibi ve çevik panoları içerir
  * [zenhub.com](https://www.zenhub.com) - GitHub'un içindeki tek proje yönetimi çözümü. Halka açık depolar, OSS ve kar amacı gütmeyen kuruluşlar için ücretsiz
  * [zenkit.com](https://zenkit.com) - Proje yönetimi ve işbirliği aracı. 5 üyeye kadar ücretsiz, 5 GB ek.
  * [Zube](https://zube.io) - 4 Proje ve 4 kullanıcı için ücretsiz planla proje yönetimi. GitHub entegrasyonu mevcuttur.

**[⬆️Başa Dön](#table-of-contents)**

## Storage and Media Processing

  * [AndroidFileHost](https://androidfilehost.com/) - Sınırsız hız, bant genişliği, dosya sayısı, indirme sayısı vb. ile ücretsiz dosya paylaşım platformu. Esas olarak APK oluşturma, özel ROM ve değişiklikler vb. gibi Android geliştirmeyle ilgili dosyalara yöneliktir. Ancak diğer dosyaları da kabul ediyor gibi görünüyor.
  * [borgbase.com](https://www.borgbase.com/) - Borg Backup için basit ve güvenli site dışı yedek barındırma. 10 GB boş yedekleme alanı ve iki depo.
  * [cloudinary.com](https://cloudinary.com/) - Ruby, Python, Java, PHP, Objective-C ve daha fazla kitaplık ile siteler ve uygulamalar için görüntü yükleme, güçlü manipülasyonlar, depolama ve dağıtım. Ücretsiz katman 25 aylık kredi içerir. Bir kredi, 1.000 görüntü dönüşümüne, 1 GB depolama alanına veya 1 GB CDN kullanımına eşittir.
  * [degoo.com](https://degoo.com/) - 20 GB'a kadar ücretsiz, üç cihaz, 5 GB yönlendirme bonusu (90 gün hesap hareketsizliği) ile yapay zeka tabanlı bulut depolama alanı.
  * [Dropshare](https://dropsha.re) - Sıfır bilgili dosya paylaşımı. AES-256-GCM şifreleme, istemci tarafı işleme ve sıfır sunucu tarafı veri erişimi ile uçtan uca şifrelenmiş dosya paylaşımı. Veri toplama gerektirmeden 1 GB'a kadar dosyalar için ücretsiz yüklemeler.
  * [embed.ly](https://embed.ly/) - Bir web sayfasına medya yerleştirmek, duyarlı görüntü ölçeklendirmek ve bir web sayfasından öğeler çıkarmak için API'ler sağlar. Saniyede 15 istekle ayda 5.000 URL'ye kadar ücretsiz
  * [Ente](https://ente.io/) - Ente, fotoğraflar, videolar ve 2FA sırları için uçtan uca şifrelenmiş bir buluttur. Ayrıca, 10 GB'lık cömert sonsuza kadar ücretsiz kullanımla birlikte kendi kendine barındırılabilir. Ücretsiz kullanım kullanıcıları için verilerin yalnızca tek bir kopyası tutulur.
  * [FileShot.io](https://fileshot.io) - Sıfır bilgiyle şifrelenmiş dosya paylaşımı. AES-256-GCM tarayıcı tarafı şifrelemesi, dosyaların yüklemeden önce tarayıcıda şifrelenmesini sağlar. Gönderen veya alıcı için hesap gerekmez. Kendi kendine barındırılabilir (MIT açık kaynak). Ücretsiz katman, dosya boyutu kısıtlaması olmaksızın sınırsız yükleme içerir.
  * [file.io](https://www.file.io) - 2 GB dosya depolama alanı. Bir dosya bir kez indirildikten sonra otomatik olarak silinir. Depolamayla etkileşim kurmak için REST API. Hız sınırı bir istek/dakikadır.
  * [freetools.site](https://freetools.site/) - Ücretsiz çevrimiçi araçlar. Belgeleri, görüntüleri, sesleri, videoları ve daha fazlasını dönüştürün veya düzenleyin.
  * [getpantry.cloud](https://getpantry.cloud/) - Kişisel projeler, hackathon'lar ve mobil uygulamalar için mükemmel olan basit bir JSON veri depolama API'si!
  * [GoFile.io](https://gofile.io/) - Ücretsiz dosya paylaşım ve depolama platformu, web tabanlı kullanıcı arayüzü ve ayrıca API aracılığıyla kullanılabilir. sınırsız dosya boyutu, bant genişliği, indirme sayısı vb. Ancak bir dosya etkin olmadığında (on günden fazla indirme yapılmadığında) silinecektir.
  * [gumlet.com](https://www.gumlet.com/) - CDN aracılığıyla resim ve video barındırma, işleme ve yayınlama. Videolar için ayda 250 GB ve görüntüler için ayda 30 GB cömert ücretsiz katman sağlar.
  * [icedrive.net](https://www.icedrive.net/) - Basit bulut depolama hizmeti. 10 GB ücretsiz depolama alanı
  * [image-charts.com](https://www.image-charts.com/) - Filigranla sınırsız resim grafiği oluşturma
  * [ImageEngine](https://imageengine.io/) - ImageEngine, kullanımı kolay bir global resim CDN'sidir. 60 saniyenin altında kurulum. AVIF ve JPEGXL desteği, WordPress-, Magento-, React-, Vue- eklentileri ve daha fazlası. Ücretsiz geliştirici hesabınızı [buradan](https://imageengine.io/developer-program/) talep edin.
  * [imagekit.io](https://imagekit.io) - Otomatik optimizasyona, gerçek zamanlı dönüşüme ve dakikalar içinde mevcut kurulumla entegre edebileceğiniz depolamaya sahip görüntü CDN'si. Ücretsiz plan ayda 20 GB'a kadar bant genişliği içerir.
  * [ImgBB](https://imgbb.com/) - ImgBB sınırsız bir resim barındırma hizmetidir. Resminizi ekranın herhangi bir yerine sürükleyip bırakın. 32 MB / resim sınırı. Görüntüyü yükledikten sonra Doğrudan görüntü bağlantılarını, BBCode ve HTML küçük resimlerini alın. Yükleme geçmişini görmek için giriş yapın.
  * [Imgbot](https://github.com/marketplace/imgbot) - Imgbot, görsellerinizi optimize eden ve size zaman kazandıran kullanıcı dostu bir robottur. Optimize edilmiş görüntüler, kaliteden ödün vermeden daha küçük dosya boyutları anlamına gelir. Açık kaynak için ücretsizdir.
  * [imgen](https://www.jitbit.com/imgen/) - Ücretsiz, sınırsız sosyal kapak görseli oluşturma API'si, filigran yok
  * [imgix](https://www.imgix.com/) - Görüntü Önbelleğe Alma, yönetim ve CDN. Ücretsiz planda 1000 kaynak görsel, sonsuz dönüşüm ve 100 GB bant genişliği bulunur
  * [internxt.com](https://internxt.com) - Internxt Drive, mutlak gizliliğe ve tavizsiz güvenliğe dayanan sıfır bilgili bir dosya depolama hizmetidir. Kaydolun ve sonsuza kadar ücretsiz 10 GB kazanın!
  * [kraken.io](https://kraken.io/) - Hizmet olarak web sitesi performansı için görsel optimizasyonu, 1 MB dosya boyutuna kadar ücretsiz plan
  * [LibreQR](https://libreqr.com) - Gizliliğe odaklanan ve takip gerektirmeyen ücretsiz QR kod oluşturucu. Veri toplamaya gerek kalmadan kullanımı ücretsizdir.
  * [MConverter](https://mconverter.eu/) - Dosyaları toplu olarak dönüştürün. [AVIF](https://mconverter.eu/convert/to/avif/) ve JXL dahil olmak üzere birçok formatı destekler. Videolardan resim çerçevelerini çıkarın. PDF'leri sıkıştırın. Sekizli gruplar halinde işlenen, her biri 100 MB'a kadar olmak üzere 24 saatte 15 dosya için ücretsiz.
  * [nitropack.io](https://nitropack.io/) - Tam ön uç optimizasyonu (önbelleğe alma, resimler ve kod optimizasyonu, CDN) ile sitenizin otomatik pilotta hızını artırın. Ayda 5.000 sayfa görüntülemeye kadar ücretsiz
  * [npoint.io](https://www.npoint.io/) - İşbirliğine dayalı şema düzenleme özelliğine sahip JSON mağazası
  * [MantleDB](https://mantledb.sh) - Komut dosyaları ve küçük uygulamalar için anonim JSON depolama alanı. Kayıt olmanıza gerek yok; güncellemeler için Master AID'yi ve genel alım için Salt Okunur RID'yi kullanır. Ücretsiz katman, 72 saatlik hareketsizlik temizleme politikasına sahip 1 paket (1 MB sınır) içerir.
  * [otixo.com](https://www.otixo.com/) - Tüm bulut depolama dosyalarınızı tek bir yerden şifreleyin, paylaşın, kopyalayın ve taşıyın. Temel plan maksimum 250 MB ile sınırsız dosya aktarımı sağlar. dosya boyutundadır ve beş şifrelenmiş dosyaya izin verir
  * [packagecloud.io](https://packagecloud.io/) - YUM, APT, RubyGem ve PyPI için Barındırılan Paket Depoları.  Sınırlı ücretsiz planlar ve açık kaynaklı planlar istek üzerine mevcuttur
  * [pcloud.com](https://www.pcloud.com/) - Bulut depolama hizmeti. 10 GB'a kadar ücretsiz depolama alanı
  * [Pinata IPFS](https://pinata.cloud) - Pinata, dosyaları IPFS'ye yüklemenin ve yönetmenin en basit yoludur. Kullanıcı dostu arayüzümüz ve IPFS API'miz Pinata'yı platformlar, yaratıcılar ve koleksiyoncular için en kolay IPFS sabitleme hizmeti haline getiriyor. API erişimiyle birlikte 1 GB ücretsiz depolama alanı.
  * [plot.ly](https://plot.ly/) - Verilerinizin grafiğini çıkarın ve paylaşın. Ücretsiz katmanda sınırsız genel dosya ve on özel dosya bulunur
  * [podio.com](https://podio.com/) - Podio'yu en fazla beş kişilik bir ekiple kullanabilir ve Temel Planın kullanıcı yönetimi dışındaki özelliklerini deneyebilirsiniz
  * [Proton Drive](https://proton.me/drive) - Dosyalar ve önemli belgeler için ultra güvenli bulut depolama. Ücretsiz plan 5 GB depolama alanı sunar.
  * [QRME.SH](https://qrme.sh) - Hızlı, güzel toplu QR kodu oluşturucu - oturum açma yok, filigran yok, reklam yok. Toplu dışa aktarma başına en fazla 100 URL.
  * [QRtracer](https://qrtracer.io) - Yerleşik tarama analitiği, toplu oluşturma ve marka özelleştirme özelliklerine sahip, herhangi bir reklam olmadan güvenilirliğe odaklanan ücretsiz QR kod oluşturucu.
  * [QuickChart](https://quickchart.io) - Yerleştirilebilir resim tabloları, grafikler ve QR kodları oluşturun
  * [redbooth.com](https://redbooth.com) - P2P dosya senkronizasyonu, 2 kullanıcıya kadar ücretsiz
  * [resmush.it](https://resmush.it) - reSmush.it, görüntü optimizasyonu sağlayan ÜCRETSİZ bir API'dir. reSmush.it, WordPress, Drupal veya Magento gibi en yaygın CMS'de uygulanmıştır. reSmush.it, hali hazırda işlenen yedi milyardan fazla görselle en çok kullanılan görsel optimizasyon API'sidir ve hala ücretsizdir.
  * [sirv.com](https://sirv.com/) - Anında görüntü optimizasyonu ve yeniden boyutlandırma özelliğine sahip Akıllı Görüntü CDN'si. Ücretsiz katman 500 MB depolama alanı ve 2 GB bant genişliği içerir.
  * [SlingSite](https://slingsite.github.io) - Resimlerinizin ve videolarınızın tüm optimize edilmiş sürümlerini oluşturun. Ücretsiz. Toplu olarak. Her görüntü için aşağıdaki formatları elde edersiniz: Seçilen üç çözünürlükte (masaüstü, tablet, mobil) AVIF, WEBP ve JPG. Videolar için şunları elde edersiniz: WebM (codec VP9), MP4 (codec HEVC aka H.265) ve MP4 (codec AVC aka H.264) artı ilk kareyle birlikte kapak resmi.
  * [sync.com](https://www.sync.com/) - Uçtan Uca bulut depolama hizmeti. 5 GB ücretsiz depolama alanı
  * [tinypng.com](https://tinypng.com/) - PNG ve JPEG görsellerini sıkıştırmak ve yeniden boyutlandırmak için kullanılan API, her ay ücretsiz 500 sıkıştırma sunar
  * [transloadit.com](https://transloadit.com/) - Dosya yüklemeyi ve video, ses, resim ve belgelerin kodlanmasını yönetir. GitHub Öğrenci Geliştirici Paketi aracılığıyla Açık kaynak, hayır kurumları ve öğrenciler için ücretsiz. Ticari uygulamalara test sürüşü için 2 GB ücretsiz alan veriliyor
  * [twicpics.com](https://www.twicpics.com) - Bir hizmet olarak duyarlı görüntüler. Görüntü optimizasyonunu otomatikleştirmek için bir görüntü CDN'si, bir medya işleme API'si ve bir ön uç kitaplığı sağlar. Hizmet, ayda 3 GB'a kadar trafik için ücretsizdir.
  * [uploadcare.com](https://uploadcare.com/hub/developers/) - Uploadcare, medya hattına en son algoritmaları temel alan en üst düzey araç setini sağlar. Tüm özellikler geliştiricilere tamamen ücretsiz olarak sunulmaktadır: Dosya Yükleme API'si ve Kullanıcı Arayüzü, Görüntü CDN'si ve Kaynak Hizmetleri, Uyarlanabilir Teslimat ve Akıllı Sıkıştırma. Ücretsiz katmanda 3000 yükleme, 3 GB trafik ve 3 GB depolama alanı bulunur.
  * [VaocherApp QR Code Generator](https://www.vaocherapp.com/qr-code-generator) - Hediye kartları, hediye çekleri ve promosyonlar için kolayca özel QR kodları oluşturun. Özel stil, renk, logo desteği...

**[⬆️Başa Dön](#table-of-contents)**

## Design and UI

  * [BoxySVG](https://boxy-svg.com) - SVG çizmek ve SVG, PNG, jpeg ve diğer formatlarda dışa aktarmak için ücretsiz, kurulabilir bir Web uygulaması.
  * [Takvim Simgeleri Oluşturucu](https://calendariconsgenerator.app/) - Tek bir tıklamayla tüm bir yılın benzersiz simgelerini tamamen ÜCRETSİZ olarak oluşturun
  * [Canva](https://canva.com) - Görsel içerik oluşturmak için ücretsiz çevrimiçi tasarım aracı.
  * [CodedThemes](https://codedthemes.com/) - Modern web geliştirmeyi basitleştirmek ve hızlandırmak için tasarlanmış, iyi hazırlanmış bir yönetici paneli ve kullanıcı arayüzü kitleri sunar.
  * [Excalidraw](https://excalidraw.com/) - Yerele ve ihracata ücretsiz kaydetme desteğine sahip ücretsiz bir çevrimiçi çizim belgesi web sayfası.
  * [figma.com](https://www.figma.com) - Ekipler için çevrimiçi, ortak çalışmaya dayalı tasarım aracı; ücretsiz katman, maksimum 2 düzenleyici ve üç projeye sahip sınırsız dosya ve görüntüleyici içerir.
  * [Flows](https://flows.sh/) - İlk katılım ve kullanıcı etkileşimi deneyimleri oluşturmak için tamamen özelleştirilebilir bir ürün benimseme platformu. Aylık olarak takip edilen 250 kullanıcıya kadar ücretsizdir.
  * [landen.co](https://www.landen.co) - Girişiminiz için güzel web siteleri ve açılış sayfaları oluşturun, düzenleyin ve yayınlayın. Hepsi kodsuz. Ücretsiz katman, tamamen özelleştirilebilir ve web'de yayınlanabilen tek bir web sitesine sahip olmanızı sağlar.
  * [lensdump.com](https://lensdump.com/) - Ücretsiz bulut resim barındırma.
  * [Logo.dev](https://www.logo.dev) - 44 milyondan fazla markaya sahip şirket logosu API'si, bir URL'yi çağırmak kadar kolaydır. İlk 10.000 API çağrısı ücretsizdir.
  * [marvelapp.com](https://marvelapp.com/) - Tasarım, prototip oluşturma ve işbirliği, tek kullanıcı ve projeyle sınırlı ücretsiz plan.
  * [Mindmup.com](https://www.mindmup.com/) - Ücretsiz olarak sınırsız zihin haritaları ve bunları bulutta saklayın. Zihin haritalarınıza her yerden, anında, herhangi bir cihazdan ulaşabilirsiniz.
  * [Mockplus iDoc](https://www.mockplus.com/idoc) - Mockplus iDoc, güçlü bir tasarım işbirliği ve aktarma aracıdır. Ücretsiz Plan, tüm özelliklerin mevcut olduğu üç kullanıcı ve beş proje içerir.
  * [Modeldraw.com](https://modeldraw.com) - UML, sistem mimarisi, akış şemaları, zihin haritaları ve Çevik iş akışlarıyla eksiksiz diyagram oluşturma platformu. Sınırsız ekip üyesiyle gerçek zamanlı işbirliği, kredi kartı gerekmez.
  * [photopea.com](https://www.photopea.com) - PSD, XCF ve Sketch formatlarını (Adobe Photoshop, Gimp ve Sketch Uygulaması) destekleyen Adobe Photoshop kullanıcı arayüzüne sahip Ücretsiz, Gelişmiş çevrimiçi tasarım düzenleyici.
  * [Plasmic](https://www.plasmic.app/) - Kod tabanınıza entegre olan hızlı, kullanımı kolay, sağlam bir web tasarım aracı ve sayfa oluşturucu. Duyarlı sayfalar veya karmaşık bileşenler oluşturun; isteğe bağlı olarak kodla genişletin; ve üretim sitelerinde ve uygulamalarda yayınlayın.
  * [Proto.io](https://www.proto.io) - Kodlamaya gerek kalmadan tamamen etkileşimli kullanıcı arayüzü prototipleri oluşturun. Ücretsiz deneme süresi sona erdiğinde ücretsiz katman kullanılabilir. Ücretsiz katman, bir kullanıcı, bir proje, beş prototip, 100 MB çevrimiçi depolama alanı ve proto.io uygulamasının bir önizlemesini içerir.
  * [Quant Ux](https://quant-ux.com/) - Quant Ux bir prototip oluşturma ve tasarım aracıdır. - Tamamen ücretsiz ve aynı zamanda açık kaynaktır.
  * [Shadcn Studio](https://shadcnstudio.com/theme-editor) - Farklı bileşenler ve düzenlerdeki tema değişikliklerinizi önizleyin.
  * [smartmockups.com](https://smartmockups.com/) - Ürün maketleri oluşturun, 200 ücretsiz maket.
  * [TeleportHQ](https://teleporthq.io/) - Az Kodlu Ön Uç Tasarım ve Geliştirme Platformu. TeleportHQ, başsız statik web sitelerini anında oluşturmak ve yayınlamak için işbirliğine dayalı bir ön uç platformdur. Üç ücretsiz proje, sınırsız ortak çalışan ve ücretsiz kod aktarımı.
  * [Unicorn Platform](https://unicornplatform.com/) - Barındırma özellikli zahmetsiz açılış sayfası oluşturucu. Ücretsiz bir web sitesi.
  * [Updrafts.app](https://updrafts.app) - Kuyruk rüzgarı tabanlı tasarımlar için WYSIWYG web sitesi oluşturucusu. Ticari olmayan kullanım için ücretsizdir.
  * [Webflow](https://webflow.com) - Animasyonlar ve web sitesi barındırma özelliğine sahip WYSIWYG web sitesi oluşturucu. İki proje için ücretsiz.
  * [Webstudio](https://webstudio.is/) - Webflow'a açık kaynaklı alternatif. Ücretsiz plan, etki alanlarında sınırsız web sitesi sunar. Özel alan adlarına sahip beş web sitesi. Ayda on bin sayfa görüntüleme. 2 GB varlık depolama alanı.
  * [whimsical.com](https://whimsical.com/) - İşbirliğine dayalı akış şemaları, tel çerçeveler, yapışkan notlar ve zihin haritaları. 4 adede kadar ücretsiz pano oluşturun.
  * [Zeplin](https://zeplin.io/) - Tasarımcı ve geliştirici işbirliği platformu. Tasarımları, varlıkları ve stil kılavuzlarını gösterin. Bir proje için ücretsiz.

**[⬆️Başa Dön](#table-of-contents)**

## Data Visualization on Maps

  * [Clockwork Micro](https://clockworkmicro.com/) - Saat gibi çalışan harita araçları. Elli bin ücretsiz aylık sorgu (harita döşemeleri, db2vector, yükseklik).
  * [Foursquare](https://developer.foursquare.com/) - Places API ve Pilgrim SDK'dan konum keşfi, mekan arama ve bağlama duyarlı içerik.
  * [geoapify.com](https://www.geoapify.com/) - Vektör ve raster harita döşemeleri, coğrafi kodlama, yerler, yönlendirme, izolin API'leri. Günde üç bin ücretsiz istek.
  * [geocod.io](https://www.geocod.io/) - API veya CSV Yükleme yoluyla coğrafi kodlama. Günde iki bin beş yüz ücretsiz sorgu.
  * [geocodify.com](https://geocodify.com/) - API veya CSV Yükleme aracılığıyla Coğrafi Kodlama ve Coğrafi Ayrıştırma. Ayda 10 bin ücretsiz sorgu.
  * [geojs.io](https://www.geojs.io/) - Yüksek düzeyde kullanılabilir REST/JSON/JSONP IP Coğrafi Konum arama API'si.
  * [Geokeo api](https://geokeo.com) - Dil düzeltme ve daha fazlasını içeren coğrafi kodlama API'si. Dünya çapında kapsama alanı. 2.500 ücretsiz günlük sorgu
  * [graphhopper.com](https://www.graphhopper.com/) - Yönlendirme, Rota için ücretsiz bir geliştirici paketi sunulmaktadır
Optimizasyon, Mesafe Matrisi, Coğrafi Kodlama ve Harita Eşleştirme.
  * [burada](https://developer.here.com/) - Haritalar ve konuma duyarlı uygulamalar için API'ler ve SDK'lar. Ayda 250 bin işlem ücretsiz.
  * [IP Coğrafi Konumu](https://ipgeolocation.io/) - Aylık 30.000 istekle ücretsiz DEVELOPER planı mevcuttur.
  * [ipstack](https://ipstack.com/) - Web Sitesi Ziyaretçilerini IP Adresine göre bulun ve tanımlayın
  * [locationiq.com](https://locationiq.com/) - Coğrafi Kodlama, Haritalar ve Yönlendirme API'leri. Beş bin istek/gün ücretsiz.
  * [mapbox.com](https://www.mapbox.com/) - Harita verilerini görüntülemek için haritalar, jeouzaysal hizmetler ve SDK'lar.
  * [maps.stamen.com](http://maps.stamen.com/) - Ücretsiz harita döşemeleri ve döşeme barındırma.
  * [maptiler.com](https://www.maptiler.com/cloud/) - Harita görselleştirmesi için vektör haritalar, harita hizmetleri ve SDK'lar. Haftalık güncellemeler ve dört harita stili içeren ücretsiz vektör döşemeleri.
  * [nominatim.org](https://nominatim.org/) - OpenStreetMap'in ücretsiz coğrafi kodlama hizmeti, küresel adres arama işlevi ve ters coğrafi kodlama yetenekleri sağlar.
  * [opencagedata.com](https://opencagedata.com) - OpenStreetMap ve diğer açık coğrafi kaynakları toplayan coğrafi kodlama API'si. Günde iki bin beş yüz ücretsiz sorgu.
  * [osmnames](https://osmnames.org/) - Coğrafi kodlama, ilgili Vikipedi sayfasının popülerliğine göre sıralanan arama sonuçları.
  * [positionstack](https://positionstack.com/) - Küresel yerler ve koordinatlar için ücretsiz coğrafi kodlama. Kişisel kullanım için ayda 25.000 İstek.
  * [stadiamaps.com](https://stadiamaps.com/) - Harita döşemeleri, yönlendirme, gezinme ve diğer coğrafi API'ler. Ticari olmayan kullanım ve test için günde iki bin beş yüz ücretsiz harita görünümü ve API isteği.

**[⬆️Başa Dön](#table-of-contents)**

## Package Build System

  * [build.opensuse.org](https://build.opensuse.org/) - Birden fazla dağıtım için paket oluşturma hizmeti (SUSE, EL, Fedora, Debian, vb.).
  * [copr.fedorainfracloud.org](https://copr.fedorainfracloud.org) - Fedora ve EL için sahte tabanlı RPM oluşturma hizmeti.
  * [help.launchpad.net](https://help.launchpad.net/Packaging) - Ubuntu ve Debian hizmeti oluşturur.

**[⬆️Başa Dön](#table-of-contents)**

## IDE and Code Editing

  * [Android Studio](https://developer.android.com/studio) - Android Studio, her tür Android cihazda uygulama oluşturmak için en hızlı araçları sağlar. Açık Kaynak IDE herkes için ücretsizdir ve en iyi Android uygulama geliştirmesidir. Windows, Mac, Linux ve hatta ChromeOS için kullanılabilir!
  * [AndroidIDE](https://m.androidide.com/) - Android cihazlarda gerçek, Gradle tabanlı Android uygulamaları geliştirmek için Açık Kaynaklı bir IDE.
  * [Apache Netbeans](https://netbeans.apache.org/) - Geliştirme Ortamı, Araç Platformu ve Uygulama Çerçevesi.
  * [apiary.io](https://apiary.io/) - Anında API modeli ve oluşturulan belgelerle ortak tasarım API'si (Tek yönetici hesabı ve barındırılan belgelerle sınırsız API planları ve sınırsız kullanıcı için ücretsiz).
  * [BBEdit](https://www.barebones.com/) - BBEdit, macOS için popüler ve genişletilebilir bir düzenleyicidir. Serbest Mod, [güçlü bir temel özellik kümesi](https://www.barebones.com/products/bbedit/comparison.html) ve gelişmiş özelliklere yükseltme yolu sağlar.
  * [Binder](https://mybinder.org/) - Git deposunu etkileşimli not defterlerinden oluşan bir koleksiyona dönüştürün. Ücretsiz bir kamu hizmetidir.
  * [BlueJ](https://bluej.org) - Yeni başlayanlar için tasarlanmış, dünya çapında milyonlarca kişi tarafından kullanılan ücretsiz bir Java Geliştirme Ortamı. Yeni başlayanlara yardımcı olmak için Oracle ve basit GUI tarafından desteklenmektedir.
  * [Bootify.io](https://bootify.io/) - Özel veritabanına ve REST API'ye sahip Spring Boot uygulama oluşturucu.
  * [Brackets](http://brackets.io/) - Brackets, özellikle web geliştirme için tasarlanmış açık kaynaklı bir metin düzenleyicisidir. Hafiftir, kullanımı kolaydır ve son derece özelleştirilebilirdir.
  * [cacher.io](https://www.cacher.io) - Etiketlere sahip ve 100'den fazla programlama dilini destekleyen kod pasajı düzenleyicisi.
  * [cocalc.com](https://cocalc.com/) - (eski adıyla cloud.sagemath.com'da SageMathCloud) - Bulutta ortak hesaplama. Yerleşik işbirliği ve matematik, bilim, veri bilimi için önceden yüklenmiş birçok ücretsiz yazılımla tam Ubuntu'ya tarayıcı erişimi: Python, LaTeX, Jupyter Notebooks, SageMath, sciktlearn, vb.
  * [code.cs50.io](https://code.cs50.io/) - Visual Studio Code for CS50, code.cs50.io adresinde bulunan ve GitHub Kod Alanlarını öğrenciler ve öğretmenler için uyarlayan bir web uygulamasıdır.
  * [Code::Blocks](https://codeblocks.org) - Ücretsiz Fortran ve C/C++ IDE. Açık Kaynaktır ve Windows, macOS ve Linux'ta çalışır.
  * [codepen.io](https://codepen.io/) - CodePen, web'in ön uç tarafı için bir oyun alanıdır.
  * [codesandbox.io](https://codesandbox.io/) - React, Vue, Angular, Preact ve daha fazlası için Çevrimiçi Oyun Alanı.
  * [codiga.io](https://codiga.io/) - Kod parçacıklarını doğrudan IDE'nizde aramanıza, tanımlamanıza ve yeniden kullanmanıza olanak tanıyan Kodlama Asistanı. Bireysel ve küçük organizasyonlar için ücretsizdir.
  * [Components.studio](https://webcomponents.dev/) - Bileşenleri ayrı ayrı kodlayın, bunları hikayelerde görselleştirin, test edin ve npm'de yayınlayın.
  * [Eclipse Che](https://www.eclipse.org/che/) - Çoklu dil desteğine sahip Geliştirici Ekipleri için Web tabanlı ve Kubernetes Yerel IDE. Açık Kaynak ve topluluk odaklı. Red Hat tarafından barındırılan çevrimiçi bir örneğe [workspaces.openshift.com](https://workspaces.openshift.com/) adresinden ulaşılabilir.
  * [ForgeCode](https://forgecode.dev/) - Claude, GPT4 Serisi, Grok, Deepseek, Gemini ve tüm sınır modelleri için yapay zeka destekli çift programcı. CLI'nizle yerel olarak çalışır ve herhangi bir IDE ile sorunsuz bir şekilde bütünleşir. Ücretsiz katman, yerel işlemeyle temel yapay zeka modeli erişimini içerir.
  * [GetVM](https://getvm.io) - Anında ücretsiz Linux ve IDE'ler krom kenar çubuğu. Ücretsiz katman günde 5 VM içerir.
  * [JDoodle](https://www.jdoodle.com) - Günde 200 krediye kadar derleyen REST API kodu için ücretsiz bir planla 60'tan fazla programlama dili için çevrimiçi derleyici ve düzenleyici.
  * [jetbrains.com](https://jetbrains.com/products.html) - Üretkenlik araçları, IDE'ler ve dağıtım araçları (diğer adıyla [IntelliJ IDEA](https://www.jetbrains.com/idea/), [PyCharm](https://www.jetbrains.com/pycharm/), vb.). Öğrenciler, öğretmenler, Açık Kaynak ve kullanıcı grupları için ücretsiz lisans.
  * [JSONPlaceholder](https://jsonplaceholder.typicode.com/) - Bazı sahte verileri döndüren bazı REST API uç noktaları
JSON biçimi. Sunucuyu yerel olarak çalıştırmak istiyorsanız kaynak kodu da mevcuttur.
  * [Lazarus](https://www.lazarus-ide.org/) - Lazarus, Hızlı Uygulama Geliştirmeye yönelik Delphi uyumlu, çapraz platformlu bir IDE'dir.
  * [MarsCode](https://www.marscode.com/) - Yapay zeka destekli ücretsiz bulut tabanlı bir IDE.
  * [micro-jaymock](https://micro-jaymock.now.sh/) - Sahte JSON verileri oluşturmaya yönelik küçük API taklit mikro hizmeti.
  * [mockable.io](https://www.mockable.io/) - Mockable, RESTful API veya SOAP web hizmetlerini taklit etmek için basit yapılandırılabilir bir hizmettir. Bu çevrimiçi hizmet, REST API veya SOAP uç noktalarını hızlı bir şekilde tanımlamanıza ve bunların JSON veya XML verilerini döndürmesini sağlamanıza olanak tanır.
  * [mockaroo](https://mockaroo.com/) - Mockaroo, CSV, JSON, SQL ve Excel formatlarında gerçekçi test verileri oluşturmanıza olanak tanır. Ayrıca arka uç API'si için örnekler de oluşturabilirsiniz.
  * [Mocklets](https://mocklets.com) - ömür boyu ücretsiz katmanla daha hızlı paralel geliştirme ve daha kapsamlı testler için API'lerin simüle edilmesine yardımcı olan HTTP tabanlı bir sahte API simülatörü.
  * [OneCompiler](https://onecompiler.com/) - Java, Python, C++, JavaScript dahil 70'ten fazla dili destekleyen ücretsiz çevrimiçi derleyici.
  * [OnlineGDB](https://onlinegdb.com) - 40'tan fazla dili destekleyen ve tonlarca kitaplıkla önceden yüklenmiş olan ücretsiz bir çevrimiçi ide; ve ayrıca bir hata ayıklama seçeneği, bayraklar, öğreticiler ve bir QNA sayfası da var!
  * [Paiza](https://paiza.cloud/en/) - Hiçbir şey ayarlamanıza gerek kalmadan Tarayıcıda Web uygulamaları geliştirin. Ücretsiz Plan, 2 CPU çekirdeği, 2 GB RAM ve 1 GB depolama alanıyla 24 24 saatlik kullanım ömrüne ve günde 4 saat çalışma süresine sahip bir sunucu sunar.
  * [PHPSandbox](https://phpsandbox.io/) - PHP için çevrimiçi geliştirme ortamı
  * [Replit](https://replit.com/) - Çeşitli program dilleri için bir bulut kodlama ortamı.
  * [SoloLearn](https://code.sololearn.com) - Kod parçacıklarını çalıştırmak için çok uygun bir bulut programlama oyun alanı. Çeşitli programlama dillerini destekler. Kodu çalıştırmak için kayıt gerekli değildir, ancak kodu platformlarına kaydederken gereklidir. Ayrıca yeni başlayanlar ve orta seviye kodlayıcılar için ücretsiz kurslar sunar.
  * [stackblitz.com](https://stackblitz.com/) - Tam yığın uygulamaları oluşturmak, düzenlemek ve dağıtmak için Çevrimiçi/Bulut Kodu IDE'si. Tüm popüler NodeJ tabanlı ön uç ve arka uç çerçevelerini destekleyin. Yeni bir proje oluşturmak için kısa bağlantı: [https://node.new](https://node.new).
  * [Sublime Text](https://www.sublimetext.com/) - Sublime Text, kodlama ve metin düzenleme görevleri için kullanılan popüler, çok yönlü ve son derece özelleştirilebilir bir metin düzenleyicisidir.
  * [Visual Studio Code](https://code.visualstudio.com/) - Kod düzenleyici, modern web ve bulut uygulamaları oluşturmak ve hata ayıklamak için yeniden tanımlandı ve optimize edildi. Microsoft tarafından geliştirildi.
  * [Visual Studio Topluluğu](https://visualstudio.microsoft.com/vs/community/) - Binlerce uzantıya sahip tam özellikli IDE, platformlar arası uygulama geliştirme (iOS ve Android için indirilebilen Microsoft uzantıları), masaüstü, web ve bulut geliştirme, çoklu dil desteği (C#, C++, JavaScript, Python, PHP ve daha fazlası).
  * [VSCodium](https://vscodium.com/) - Topluluk odaklı, telemetri/izleme olmadan ve Microsoft'un düzenleyicisi VSCode'un serbestçe lisanslanan ikili dağıtımı
  * [wakatime.com](https://wakatime.com/) - Metin düzenleyici eklentilerini kullanarak kodlama etkinliğinizle ilgili ölçülmüş öz ölçümler, sınırlı ücretsiz plan.
  * [Wave Terminali](https://waveterm.dev/) - Wave, kesintisiz iş akışları için açık kaynaklı, platformlar arası bir terminaldir. Her şeyi satır içi olarak işleyin. Oturumları ve geçmişi kaydedin. Açık web standartları tarafından desteklenmektedir. MacOS ve Linux.

**[⬆️Başa Dön](#table-of-contents)**

## Analytics, Events and Statistics

  * [amplitude.com](https://amplitude.com/) - 1 milyon aylık etkinlik, en fazla 2 uygulama
  * [AppFit](https://appfit.io) - AppFit, analizlerin ve ürün güncellemelerinin sorunsuz, platformlar arası yönetimini kolaylaştırmak için tasarlanmış kapsamlı bir analiz ve ürün yönetimi aracıdır. Ücretsiz planda ayda 10.000 etkinlik, ürün günlüğü ve haftalık bilgiler bulunur.
  * [Aptabase](https://aptabase.com) - Mobil ve Masaüstü Uygulamalar için Açık Kaynak, Gizlilik Dostu ve Basit Analiz. Swift, Kotlin, React Native, Flutter, Electron ve diğerleri için SDK'lar. Ayda 20.000'e kadar etkinlik için ücretsiz.
  * [Avo](https://avo.app/) - Basitleştirilmiş analiz yayın iş akışı. Tek kaynaklı doğruluk izleme planı, tür güvenli analitik izleme kitaplığı, uygulama içi hata ayıklayıcılar ve yayınlanmadan önce tüm veri sorunlarını yakalamak için veri gözlemlenebilirliği. İki çalışma alanı üyesi için ücretsiz ve 1 saatlik veri gözlemlenebilirliği incelemesi.
  * [Beampipe.io](https://beampipe.io) - Beampipe basit, gizlilik odaklı bir web analitiğidir. 5 alana kadar ücretsiz ve aylık 10.000 sayfa görüntüleme.
  * [Census](https://www.getcensus.com/) - Ters ETL ve Operasyonel Analitik Platformu. Veri ambarınızdaki 10 alanı Salesforce, Zendesk veya Amplitude gibi 60'tan fazla SaaS ile senkronize edin.
  * [Clicky](https://clicky.com) - Web Sitesi Analiz Platformu. 3000 görüntüleme analizine sahip bir web sitesi için Ücretsiz Plan.
  * [counter.dev](https://counter.dev) - Web analitiği basitleştirildi ve bu nedenle gizlilik dostu hale getirildi. Ücretsiz veya bağış yoluyla istediğinizi ödeyin.
  * [DocBeacon](https://docbeacon.io) - Belge izleme ve etkileşim Analytics ile güvenli belge paylaşımı. Ücretsiz plan, 20'ye kadar PDF belgesini (maks. 10 MB), 10 kişiyi ve belge başına 2 paylaşımı destekler; indirme işlemleri, zaman ve etkileşim görünümleri için temel analizlerle birlikte.
  * [Dwh.dev](https://dwh.dev) - Veri Bulutu Gözlemlenebilirliği Çözümü (Snowflake). Kişisel kullanım için ücretsizdir.
  * [Harcama](https://www.expensify.com/) - Gider raporlama, ücretsiz kişisel raporlama onayı iş akışı
  * [getinsights.io](https://getinsights.io) - Gizlilik odaklı, çerez içermeyen analizler, ayda 3 bin etkinliğe kadar ücretsiz.
  * [GoatCounter](https://www.goatcounter.com/) - GoatCounter, barındırılan bir hizmet (ticari olmayan kullanım için ücretsiz) veya kendi kendine barındırılan bir uygulama olarak sunulan açık kaynaklı bir web analizi platformudur. Google Analytics veya Matomo'ya alternatif olarak kullanımı kolay ve anlamlı gizlilik dostu web analitiği sunmayı amaçlamaktadır. Ücretsiz katman ticari olmayan kullanıma yöneliktir ve sınırsız site, altı aylık veri saklama ve ayda 100 bin sayfa görüntüleme içerir.
  * [Google Analytics](https://analytics.google.com/) - Google Analytics
  * [heap.io](https://heap.io) - iOS veya web uygulamalarındaki her kullanıcı eylemini otomatik olarak yakalar. Aylık 10.000'e kadar oturum için ücretsiz.
  * [Hightouch](https://hightouch.com/) - Hightouch, müşteri verilerini veri ambarınızdan CRM, pazarlama ve destek araçlarınıza senkronize etmenize yardımcı olan bir Ters ETL platformudur. Ücretsiz katman, verileri senkronize edebileceğiniz tek bir hedef sunar.
  * [Hotjar](https://hotjar.com) - Web Sitesi Analizleri ve Raporlar . Ücretsiz Plan günde 2000 sayfa görüntülemeye izin verir. Yüz anlık görüntü/gün (maks. kapasite: 300). Üç anlık görüntü ısı haritası 365 gün boyunca saklanabilir. Sınırsız Ekip Üyesi. Ayrıca Uygulamada ve bağımsız anketlerde, ekran görüntülerini içeren geri bildirim widget'ları. Ücretsiz katman, 3 anket ve 3 geri bildirim widget'ı oluşturmaya ve ayda 20 yanıt toplamaya olanak tanır.
  * [LogSpot](https://logspot.io) - Yerleştirilebilir analiz araçları ve otomatik robotlar (slack, telgraf ve web kancaları) dahil olmak üzere tam birleştirilmiş web ve ürün analizi platformu. Ücretsiz plan ayda 10.000 etkinlik içerir.
  * [MetricsWave](https://metricswave.com) - Geliştiriciler için gizlilik dostu Google Analytics alternatifi. Ücretsiz plan, kredi kartı gerektirmeden ayda 1 milyon sayfa görüntülemeye izin verir.
  * [Mixpanel](https://mixpanel.com/) - 100.000 aylık takip edilen kullanıcı, sınırsız veri geçmişi ve koltuklar, ABD veya AB veri yerleşimi
  * [Moesif](https://www.moesif.com) - REST ve GraphQL için API analitiği. (Ayda 500.000 API çağrısına kadar ücretsiz)
  * [PostHog](https://posthog.com) - Ayda 1 milyona kadar izlenen etkinlik için ücretsiz Tam Ürün Analizi paketi. Ayrıca ayda 250 yanıtla sınırsız Uygulama İçi Anketler sağlar.
  * [Repohistory](https://repohistory.com) - 14 günden daha uzun GitHub repo trafik geçmişini izlemek için güzel kontrol paneli. Ücretsiz Plan, kullanıcıların tek bir depoya yönelik trafiği izlemesine olanak tanır.
  * [Row Zero](https://rowzero.io) - Son derece hızlı, bağlantılı elektronik tablo. Veri veritabanlarına, S3'e ve API'lere doğrudan bağlanın. Milyonlarca satırı anında içe aktarın, analiz edin, grafiğini oluşturun ve paylaşın. Üç ücretsiz (sonsuza kadar) çalışma kitabı.
  * [Rybbit](https://rybbit.io) - Google Analytics'e 10 kat daha sezgisel, açık kaynaklı ve çerezsiz bir alternatif. Ücretsiz planlarda 3.000 aylık etkinlik bulunur.
  * [Seline](https://seline.so) - Seline basit ve özel bir web sitesi ve ürün analizidir. Çerezsiz, hafif, bağımsız. Ücretsiz plan ayda 3.000 etkinlik içerir ve kontrol paneli, kullanıcı yolculukları, dönüşüm hunileri ve daha fazlası gibi tüm özelliklerimize erişim sağlar.
  * [StatCounter](https://statcounter.com/) - Web Sitesi Görüntüleyici Analizi. En yeni 500 ziyaretçinin analizi için ücretsiz plan.
  * [Statsig](https://statsig.com) - Analitik, özellik işaretleme ve A/B testini kapsayan hepsi bir arada platform. Ayda 1 milyona kadar ölçümlü etkinlik için ücretsiz.
  * [TraceLog](https://tracelog.io/) - E-ticaret için AI Analytics. Analitikleriniz hakkında doğal dilde sorular sorun, uygulanabilir öneriler alın ve yapay zeka destekli bilgilerle gelirinizi artırın. Ayda 10.000'e kadar etkinlik için ücretsiz.
  * [İzlemeplanı](https://www.trackingplan.com/) - Dijital analizleri, pazarlama verilerini ve piksel sorunlarını otomatik olarak algılayın, güncel izleme planlarını sürdürün ve kusursuz işbirliğini teşvik edin. Bunu gerçek trafikle üretim ortamınıza dağıtın veya kod yazmadan regresyon testlerinize analitik kapsamı ekleyin.
  * [TrackWith Dicloud](https://dicloud.net/trackwith-privacy-focused-analytics/) - Google Analytics'e ücretsiz, hafif ve gizlilik odaklı bir alternatif. Sınırsız sayfa görüntüleme, sınırsız ziyaretçi, sınırsız sayfa ısı haritaları ve hedef izleme. En fazla 3 alan adı ve alan adı başına 600 oturum tekrarı için ücretsiz.
  * [Umami](https://umami.is/) - Google Analytics'e basit, hızlı, gizlilik odaklı, açık kaynaklı bir alternatif.
  * [usabilityhub.com](https://usabilityhub.com/) - Tasarımları ve modelleri gerçek kişiler üzerinde test edin ve ziyaretçileri takip edin. Tek kullanıcı için ücretsiz, sınırsız test
  * [Userbird](https://userbird.com) - Isı haritaları, oturum kayıtları ve gelir izleme özelliğine sahip Google Analytics alternatifi.

**[⬆️Başa Dön](#table-of-contents)**

## Visitor Session Recording

  * [FullStory.com](https://www.fullstory.com) - Bir aylık veri saklama ve üç kullanıcı koltuğuyla ayda 1.000 oturum. Daha fazla bilgi [burada](https://help.fullstory.com/hc/en-us/articles/360020623354-FullStory-Free-Edition).
  * [howuku.com](https://howuku.com) - Kullanıcı etkileşimini, katılımını ve etkinliği izleyin. Ayda 5.000 ziyarete kadar ücretsiz
  * [inspectlet.com](https://www.inspectlet.com/) - Bir web sitesi için ayda 2.500 oturum ücretsiz
  * [LogRocket.com](https://www.logrocket.com) - 30 günlük saklama, hata izleme, canlı mod ile ayda 1.000 oturum
  * [Microsoft Clarity](https://clarity.microsoft.com/) - "Trafik sınırı yok", proje sınırı yok ve örnekleme yok; tamamen ücretsiz oturum kaydı
  * [mouseflow.com](https://mouseflow.com/) - Bir web sitesi için ayda 500 oturum ücretsiz
  * [OpenReplay.com](https://www.openreplay.com) - Hataların yeniden oluşturulması için geliştirme araçları, gerçek zamanlı destek için canlı oturum ve ürün analiz paketi içeren açık kaynaklı oturum tekrarı. Tüm özelliklere erişim ve 7 günlük saklama süresiyle ayda bin oturum.
  * [Reactflow.com](https://www.reactflow.com/) - Site başına: Günde 1.000 sayfa görüntüleme, üç ısı haritası, üç widget, ücretsiz hata takibi
  * [smartlook.com](https://www.smartlook.com/) - web ve mobil uygulamalar için ücretsiz paketler (1500 oturum/ay), üç ısı haritası, bir dönüşüm hunisi, 1 aylık veri geçmişi
  * [UXtweak.com](https://www.uxtweak.com/) - Ziyaretçilerin web sitenizi veya uygulamanızı nasıl kullandıklarını kaydedin ve izleyin. Küçük projeler için ücretsiz sınırsız süre

**[⬆️Başa Dön](#table-of-contents)**

## International Mobile Number Verification API and SDK

  * [numverify](https://numverify.com/) - Genel telefon numarası doğrulama ve arama JSON API'si. 100 API isteği/ay
  * [veriphone](https://veriphone.io/) - Ücretsiz, hızlı, güvenilir bir JSON API'sinde genel telefon numarası doğrulaması. 1000 istek/ay

**[⬆️Başa Dön](#table-of-contents)**

## Payment and Billing Integration

  * [Adapty.io](https://adapty.io/) - iOS, Android, React Native, Flutter, Unity veya web uygulamasına mobil uygulama içi abonelik entegrasyonu için açık kaynaklı SDK ile tek elden çözüm. Aylık 10 bin dolara kadar ücretsiz gelir.
  * [CoinMarketCap](https://coinmarketcap.com/api/) - En son kripto ve fiat döviz kurları dahil olmak üzere kripto para piyasası verilerini sağlar. Ücretsiz katman ayda 10.000 çağrı kredisi sunar.
  * [Currencyapi](https://currencyapi.com) - Ücretsiz para birimi dönüştürme ve döviz kuru verileri API'sı. Ayda 300 istek ücretsiz, özel kullanım için dakikada 10 istek.
  * [CurrencyApi](https://currencyapi.net/) - Fiziksel ve Kripto para birimleri için JSON ve XML olarak sunulan Canlı Döviz Kurları. Ücretsiz katman ayda 1.250 API isteği sunar.
  * [CurrencyFreaks](https://currencyfreaks.com/) - Güncel ve geçmiş döviz kurlarını sağlar. Ayda 1000 istekle ücretsiz DEVELOPER planı mevcuttur.
  * [currencylayer](https://currencylayer.com/) - İşletmeniz için Güvenilir Döviz Kurları ve Para Birimi Dönüştürme, ayda 100 API isteği ücretsiz.
  * [exchangerate-api.com](https://www.exchangerate-api.com) - Kullanımı kolay bir para birimi dönüştürme JSON API'si. Ücretsiz katman, ayda 1.500 istek sınırıyla günde bir kez güncellenir.
  * [FraudLabsPRO](https://www.fraudlabspro.com) - Satıcıların ödeme sahtekarlığını ve ters ibrazları önlemelerine yardımcı olun. Ücretsiz Mikro Plan, ayda 500 sorguyla kullanılabilir.
  * [FxRatesAPI](https://fxratesapi.com) - Gerçek zamanlı ve geçmiş döviz kurlarını sağlar. Ücretsiz katman, ilişkilendirme gerektirir.
  * [Moesif API Monetization](https://www.moesif.com/) - Kullanıma dayalı faturalandırma yoluyla API'lerden gelir elde edin. Stripe, Chargebee vb.'ye bağlanın. Ücretsiz katman ayda 30.000 etkinlik sunar.
  * [ParityVend](https://www.ambeteco.com/ParityVend/) - İşletmenizi dünya çapında genişletmek ve yeni pazarlara ulaşmak için fiyatları ziyaretçinin konumuna göre otomatik olarak ayarlayın (satın alma gücü paritesi). Ücretsiz plan ayda 7.500 API isteği içerir.
  * [Qonversion](http://qonversion.io/) - Uygulama içi satın almaları ve para kazanmayı optimize etmek için analizler, A/B testleri, Apple Arama Reklamları, uzaktan yapılandırmalar ve büyüme araçları sunan hepsi bir arada platformlar arası abonelik yönetimi platformu. iOS, Android, React Native, Flutter, Unity, Cordova, Stripe ve web ile uyumludur. Aylık takip edilen gelirde 10 bin dolara kadar ücretsiz.
  * [RevenueCat](https://www.revenuecat.com/) - Uygulama içi satın almalar ve abonelikler (iOS ve Android) için barındırılan arka uç. Takip edilen gelirde ayda 2,5 bin dolara kadar ücretsiz.
  * [vatlayer](https://vatlayer.com/) - Anında KDV numarası doğrulama ve AB KDV oranları API'si, ayda 100 API isteği ücretsiz

**[⬆️Başa Dön](#table-of-contents)**

## Docker Related

  * [Konteyner Kayıt Hizmeti](https://container-registry.com/) - Liman tabanlı Konteyner Yönetim Çözümü. Ücretsiz katman, özel depolar için 1 GB depolama alanı sunar.
  * [Docker Hub](https://hub.docker.com) - Docker görüntüleri oluşturmak ve depolamak için ücretsiz bir özel depo ve sınırsız genel depo
  * [Docker ile Oynayın](https://labs.play-with-docker.com/) - Docker'ı öğrenmek için basit, etkileşimli ve eğlenceli bir oyun alanı.
  * [quay.io](https://quay.io/) - Sınırsız ücretsiz halka açık depolarla konteyner görüntüleri oluşturun ve saklayın
  * [ttl.sh](https://ttl.sh/) - Anonim ve geçici Docker görüntü kaydı

**[⬆️Başa Dön](#table-of-contents)**

## Dev Blogging Sites

  * [AyeDot](https://ayedot.com/) - Fikirlerinizi, bilgilerinizi ve hikayelerinizi Modern multimedya kısa formatlı Minibloglar biçiminde ücretsiz olarak dünyayla paylaşın.
  * [BearBlog](https://bearblog.dev/) - Minimalist, Markdown destekli blog ve web sitesi oluşturucu.
  * [Dev.to](https://dev.to/) - Programcıların fikirlerini paylaştığı ve birbirlerinin büyümesine yardımcı olduğu yer.
  * [Hashnode](https://hashnode.com/) - Geliştiriciler için Sorunsuz Bloglama Yazılımı!.
  * [Medium](https://medium.com/) - Sizin için neyin önemli olduğu konusunda daha düşünceli olun.
  * [JustBlogged](https://justblogged.com) - Özel alan adı desteğine ve hızlı küresel performansa sahip ücretsiz blog platformu.

**[⬆️Başa Dön](#table-of-contents)**

## Commenting Platforms

  * [GraphComment](https://graphcomment.com/) - GraphComment, web sitesinin hedef kitlesinden aktif bir topluluk oluşturmanıza yardımcı olan bir yorum platformudur.
  * [IntenseDebate](https://intensedebate.com/) - WordPress, Tumblr, Blogger ve diğer birçok web sitesi platformu için zengin özelliklere sahip bir yorum sistemi.
  * [Remarkbox](https://www.remarkbox.com/) - Açık kaynaklı, barındırılan yorum platformu, "Birkaç alanda davranış ve görünüm üzerinde tam kontrole sahip bir moderatör" için elinizden geleni yapın
  * [Utterances](https://utteranc.es/) - GitHub sorunları üzerine oluşturulmuş hafif bir yorum widget'ı. Blog yorumları, wiki sayfaları ve daha fazlası için GitHub konularını kullanın!

**[⬆️Başa Dön](#table-of-contents)**

## Screenshot APIs

  * [ApiFlash](https://apiflash.com) - Aws Lambda ve Chrome'u temel alan bir ekran görüntüsü API'si. Tam sayfayı yönetir, zamanlamayı ve görüntü alanı boyutlarını yakalar.
  * [microlink.io](https://microlink.io/) - Bir hizmet olarak herhangi bir web sitesini meta etiket normalleştirmesi, güzellik bağlantısı önizlemeleri, kazıma yetenekleri veya ekran görüntüleri gibi verilere dönüştürür. Her gün 250 istek/gün ücretsiz.
  * [PhantomJsCloud](https://PhantomJsCloud.com) - Tarayıcı otomasyonu ve sayfa oluşturma.  Ücretsiz Katman günde 500 sayfaya kadar baskı sunar.  2017'den beri Ücretsiz Katman.
  * [screenshotbase.com](https://screenshotbase.com) - Ayda 300 ücretsiz ekran görüntüsü. Herhangi bir URL'den ekran görüntüleri alın. Hızlı, ücretsiz ve ölçeklenebilir.
  * [screenshotlayer.com](https://screenshotlayer.com/) - Herhangi bir web sitesinin son derece özelleştirilebilir anlık görüntülerini yakalayın. Aylık ücretsiz 100 anlık görüntü
  * [screenshotmachine.com](https://www.screenshotmachine.com/) - Yalnızca ana sayfayı değil, tam uzunluktaki çekimler de dahil olmak üzere ayda 100 anlık görüntü, png, gif ve jpg yakalayın
  * [Screenshot Scout](https://screenshotscout.com/) - Geliştiriciler için ekran görüntüsü API'si. Tek bir istekte herhangi bir URL'den temiz, üretime hazır ekran görüntüleri. Ücretsiz plan, sonsuza kadar ayda 200 ekran görüntüsü içerir.
  * [SnapAPI](https://snapapi.pics) - Ekran görüntüsü, video kaydı, PDF oluşturma ve web veri çıkarma API'si. Ücretsiz plan ayda 200 ekran görüntüsü içerir.
  * [thumbnail.ws](https://thumbnail.ws) - Web sitelerinin küçük resimlerini oluşturmaya yönelik API. Ayda 1.000 istek ücretsiz.

**[⬆️Başa Dön](#table-of-contents)**

## Flutter Related and Building IOS Apps without Mac

  * [CodeMagic](https://codemagic.io/) - Codemagic, mobil uygulamalara yönelik tamamen barındırılan ve yönetilen bir CI/CD'dir. GUI tabanlı bir CI/CD aracıyla derleyebilir, test edebilir ve dağıtabilirsiniz. Ücretsiz katman, ayda 500 ücretsiz dakika ve 2,3 GHz ve 8 GB RAM'e sahip bir Mac Mini örneği sunar.
  * [FlutLab](https://flutlab.io/) - FlutLab, modern bir Flutter çevrimiçi IDE'sidir ve platformlar arası projeler oluşturmak, hata ayıklamak ve oluşturmak için en iyi yerdir. Flutter ile iOS (Mac olmadan) ve Android uygulamaları oluşturun.
  * [FlutterFlow](https://flutterflow.io/) - FlutterFlow, flutter kullanarak mobil uygulama oluşturmaya yönelik tarayıcı tabanlı bir sürükle ve bırak arayüzüdür.

**[⬆️Başa Dön](#table-of-contents)**

## Browser-based hardware emulation written in Javascript

  * [Jor1k](https://s-macke.github.io/jor1k/demos/main.html) - Linux'u ağ desteğiyle çalıştırabilen bir OpenRISC sanal makinesi.
  * [JsLinux](https://bellard.org/jslinux) - Linux ve Windows 2k çalıştırabilen gerçekten hızlı bir x86 sanal makine.
  * [v86](https://copy.sh/v86) - Linux'u ve diğer işletim sistemlerini doğrudan tarayıcıda çalıştırabilen bir x86 sanal makinesi.

**[⬆️Başa Dön](#table-of-contents)**

## Privacy Management

  * [Bearer](https://www.bearer.sh/) - Kuruluşların GDPR ve diğer düzenlemelere uyması için denetimler ve sürekli iş akışları yoluyla gizliliğin tasarım gereği uygulanmasına yardımcı olur. Ücretsiz katman yalnızca daha küçük ekiplerle ve SaaS sürümüyle sınırlıdır.
  * [Concord](https://www.concord.tech/) - İzin yönetimi, gizlilik talebi yönetimi (DSAR'lar) ve veri eşleme dahil tam veri gizliliği platformu. Ücretsiz katman, temel izin yönetimi özelliklerini içerir ve ayrıca ücretsiz ve doğrulanmış açık kaynaklı projeler için daha gelişmiş bir plan sunar.
  * [Cookiefirst](https://cookiefirst.com/) - Çerez banner'ları, denetim ve çok dilli izin yönetimi çözümü. Ücretsiz katman, tek seferlik tarama ve tek banner sunar.
  * [Iubenda](https://www.iubenda.com/) - Gizlilik ve çerez politikaları ve izin yönetimi. Ücretsiz katman, sınırlı gizlilik ve çerez politikasının yanı sıra çerez bannerları da sunar.
  * [Ketch](https://www.ketch.com/) - Rıza yönetimi ve gizlilik çerçevesi aracı. Ücretsiz katman, çoğu özelliği sınırlı bir ziyaretçi sayısıyla sunar.

**[⬆️Başa Dön](#table-of-contents)**

## Miscellaneous

  * [BackgroundStyler.com](https://backgroundstyler.com) - Sosyal medyada paylaşmak üzere kodunuzun, metninizin veya görsellerinizin estetik ekran görüntülerini oluşturun.
  * [Base64 kod çözücü/kodlayıcı](https://devpal.co/base64-decode/) - Verilerin kodunu çözmek ve kodlamak için çevrimiçi ücretsiz araç.
  * [BinShare.net](https://binshare.net) - Kod veya ikili dosyalar oluşturun ve paylaşın. Güzel bir resim olarak paylaşılabilir; Twitter / Facebook gönderisi için veya bağlantı olarak ör. sohbetler veya forumlar için.
  * [Blynk](https://blynk.io) - IoT cihazlarını kontrol etmek, oluşturmak ve değerlendirmek için API içeren bir SaaS. 5 cihaz, Ücretsiz Bulut ve veri depolama içeren Ücretsiz Geliştirici Planı. Mobil Uygulamalar da mevcuttur.
  * [Bricks Note Calculator](https://free.getbricks.app/) - güçlü yerleşik çok satırlı hesap makinesine sahip bir not alma uygulaması (PWA).
  * [Carbon.now.sh](https://carbon.now.sh) - Estetik ekran görüntüsü benzeri bir görüntü formatında kod parçacıkları oluşturun ve paylaşın. Genellikle kod parçacıklarını Twitter'da veya blog gönderilerinde estetik olarak paylaşmak/göstermek için kullanılır.
  * [Code Time](https://www.software.com/code-time) - VS Code, Atom, IntelliJ, Sublime Text ve daha fazlasındaki zaman takibi ve kodlama ölçümleri için bir uzantı.
  * [Codepng](https://www.codepng.app) - Kaynak kodunuzdan sosyal medyada paylaşmak üzere mükemmel anlık görüntüler oluşturun.
  * [CodeToImage](https://codetoimage.com/) - Sosyal medyada paylaşmak üzere kod veya metnin ekran görüntülerini oluşturun.
  * [cron-job.org](https://cron-job.org) - Çevrimiçi cronjobs hizmeti. Sınırsız işler ücretsizdir.
  * [Cronhooks](https://cronhooks.io/) - Zamanında veya yinelenen web kancaları planlayın. Ücretsiz plan 5 geçici programa izin verir.
  * [datelist.io](https://datelist.io) - Çevrimiçi rezervasyon / randevu planlama sistemi. Ayda 5 rezervasyona kadar ücretsiz, 1 takvim dahildir
  * [Alan Yönlendirme](https://domain-forward.com/) - Herhangi bir URL'yi veya Etki Alanını iletmek için basit bir araç. Ayda 5 alan adına ve 200 bin isteğe kadar ücretsiz.
  * [Exif Editor](https://exifeditor.io/) - Tarayıcıda görüntü/fotoğraf meta verilerini anında görüntüleyin, düzenleyin, fırçalayın, analiz edin - GPS konumu ve meta veriler dahil.
  * [Format Express](https://www.format-express.dev) - JSON / XML / SQL için anında çevrimiçi format.
  * [FOSSA](https://fossa.com/) - Üçüncü taraf kodu, lisans uyumluluğu ve güvenlik açıklarına yönelik ölçeklenebilir, uçtan uca yönetim.
  * [Hook Relay](https://www.hookrelay.dev/) - Sorun yaşamadan uygulamanıza webhook desteği ekleyin: sıraya alma, geri çekilmeli yeniden denemeler ve günlük kaydı sizin için yapılır. Ücretsiz planda günde 100 teslimat, 14 günlük saklama ve 3 kanca uç noktası bulunur.
  * [Barındırma Denetleyicisi](https://hostingchecker.co) - Herhangi bir alan adı, web sitesi veya IP adresi için ASN, İSS, konum ve daha fazlası gibi barındırma bilgilerini kontrol edin. Ayrıca birden fazla barındırma ve DNS ile ilgili araç içerir.
  * [newreleases.io](https://newreleases.io/) - GitHub, GitLab, Bitbucket, Python PyPI, Java Maven, Node.js NPM, Node.js Yarn, Ruby Gems, PHP Packagist, .NET NuGet, Rust Cargo ve Docker Hub'ın yeni sürümleri için e-posta, Slack, Telegram, Discord ve özel web kancalarıyla ilgili bildirimler alın.
  * [OnlineExifViewer](https://onlineexifviewer.com/) - GPS konumu ve meta verileri dahil olmak üzere bir fotoğrafın EXIF ​​verilerini anında çevrimiçi görüntüleyin.
  * [PDFMonkey](https://www.pdfmonkey.io/) - Bir kontrol panelinde PDF şablonlarını yönetin, dinamik verilerle API'yi çağırın ve PDF'nizi indirin. Ayda 300 ücretsiz belge sunar.
  * [Pika Code Screenshots](https://pika.style/templates/code-image) - Uzantıyı kullanarak kod parçacıkları ve VSCode'dan güzel, özelleştirilebilir ekran görüntüleri oluşturun.
  * [QuickType.io](https://quicktype.io/) - Herhangi bir programlama dilinde verilerle hızlı ve güvenli bir şekilde çalışmak için JSON, şema ve GraphQL'den modelleri/sınıf/tür/arabirimi ve serileştiricileri hızla otomatik olarak oluşturun. JSON'u herhangi bir dilde muhteşem, güvenli koda dönüştürün.
  * [RandomKeygen](https://randomkeygen.com/) - Herhangi bir uygulamayı, hizmeti veya cihazı güvence altına almak için kullanabileceğiniz, rastgele oluşturulmuş çeşitli anahtarlar ve şifreler sunan ücretsiz, mobil uyumlu bir araç.
  * [ray.so](https://ray.so/) - Kod parçacıklarınızın güzel resimlerini oluşturun.
  * [readme.com](https://readme.com/) - Kolaylaştırılmış güzel belgeler, Açık Kaynak için ücretsiz.
  * [redirect.pizza](https://redirect.pizza/) - HTTPS desteğiyle yönlendirmeleri kolayca yönetin. Ücretsiz plan, 10 kaynak ve ayda 100.000 isabet içerir.
  * [redirection.io](https://redirection.io/) - İşletmeler, pazarlama ve SEO için HTTP yönlendirmelerini yönetmeye yönelik SaaS aracı.
  * [Renamer.ai](https://renamer.ai) - 20'den fazla dil için OCR, meta veri çıkarma ve otomasyon özelliklerine sahip, yapay zeka destekli dosya yeniden adlandırma aracı. Ücretsiz kullanım: Masaüstü uygulaması, toplu yeniden adlandırma, otomatik yeniden adlandırma ve normal destek dahil ayda 15 dosya.
  * [ReqBin](https://reqbin.com/) - HTTP İsteklerini Çevrimiçi Gönderin. Popüler İstek Yöntemleri arasında GET, POST, PUT, DELETE ve HEAD bulunur. Başlıkları ve Belirteç Kimlik Doğrulamasını destekler. İsteklerinizi kaydetmek için temel bir giriş sistemi içerir.
  * [Smartcar API](https://smartcar.com) - Arabaların yerini tespit etmek, yakıt deposunu, pil seviyelerini, kilometre sayacını, kapıların kilidini açmak/kilitlemek vb. bilgileri almak için bir API.
  * [snappify](https://snappify.com) - Geliştiricilerin çarpıcı görseller oluşturmasına olanak tanır. Güzel kod parçacıklarından tam kapsamlı teknik sunumlara kadar. Ücretsiz plan, sınırsız indirme ile aynı anda en fazla 3 anlık görüntü ve ayda 5 yapay zeka destekli kod açıklaması içerir.
  * [Gün Doğumu ve Gün Batımı](https://sunrisesunset.io/api/) - Belirli bir boylam ve enlem için gün doğumu ve gün batımı saatlerini alın.
  * [superfeedr.com](https://superfeedr.com/) - Gerçek zamanlı PubSubHubbub uyumlu yayınlar, dışa aktarma, analizler. Daha az özelleştirme ile ücretsiz
  * [SurveyMonkey.com](https://www.surveymonkey.com) - Çevrimiçi anketler oluşturun. Sonuçları çevrimiçi analiz edin. Ücretsiz plan anket başına yalnızca 10 soru ve 100 yanıta izin verir.
  * [SYNCDATE](https://syncdate.app) - İki yönlü Google Takvim senkronizasyonu. Ücretsiz katman: 2 hesap, sınırsız etkinlik.
  * [UUID Oluşturucu](https://newuuid.com/) - Kurumsal düzeyde anında UUID v1, UUID v4, UUID v7, GUID, Nil UUID'ler, CUID v1/v2, NanoID ve ULID oluşturun
  * [Sürüm beslemeleri](https://versionfeeds.com) - Favori yazılımınızın sürümleri için özel RSS beslemeleri. Programlama dillerinizin, kitaplıklarınızın veya sevdiğiniz araçlarınızın en son sürümlerini tek bir beslemede bulundurun. (İlk 3 yayın ücretsizdir)
  * [videoinu](https://videoinu.com) - Ekran kayıtlarını ve diğer videoları çevrimiçi olarak oluşturun ve düzenleyin.
  * [Volume Shader BM](https://volumeshaderbm.org) - Ücretsiz tarayıcı tabanlı GPU karşılaştırması (WebGL). Geliştiricilerin gölgelendirici performansını tarayıcılar ve cihazlar arasında tekrarlanabilir şekilde test etmesine ve karşılaştırmasına yardımcı olur.
  * [Webacus](https://webacus.dev) - Kodlama, kod çözme ve veri işleme için çok çeşitli ücretsiz geliştirici araçlarına erişin.
  * [XKit](https://xkit.io) - Geliştiricilerin, öğrencilerin ve günlük kullanıcıların hayatını kolaylaştırmak için tasarlanmış ücretsiz çevrimiçi araçlardan oluşan bir koleksiyon. Çok çeşitli Geliştirici araçları, Fark/Karşılaştırma araçları, Hesap Makineleri, Dönüştürücüler ve Oluşturucular içerir.
performans ve güvenlik
  * [Dadroit V Web](https://dadroit.com/vweb/) - Büyük dosyalar için tarayıcı içi JSON görüntüleyici. Taşıyıcı/Temel kimlik doğrulama ile ağaç görünümü, RegEx araması, dışa aktarma ve URL yükleme. Tamamen istemci tarafında, veri yüklenmedi. Özgür.

**[⬆️Başa Dön](#table-of-contents)**

## Remote Desktop Tools

  * [AnyDesk](https://anydesk.com) - 3 cihaz için ücretsiz, oturum sayısı ve süresinde sınırlama yok
  * [Getscreen.me](https://getscreen.me) - 2 cihaz için ücretsiz, oturum sayısı ve süresinde sınırlama yok
  * [RemSupp](https://remsupp.com) - İsteğe bağlı destek ve cihazlara kalıcı erişim (günde 2 oturum ücretsiz)
  * [RustDesk](https://rustdesk.com/) - Herkes için açık kaynaklı sanal/uzak masaüstü altyapısı!

**[⬆️Başa Dön](#table-of-contents)**

## Game Development

  * [3Dassets.one](https://3dassets.one/) - 8.000'den fazla ücretsiz/ücretli 3D model ve doku oluşturmaya yönelik PBR malzemeleri.
  * [ArtStation](https://www.artstation.com/) - Ücretsiz/Ücretli 2D, 3D varlıklar ve sesler, simgeler, döşeme setleri, oyun kitleri için MarketPlace. Ayrıca sanat portföyünüzü sergilemek için de kullanılabilir.
  * [CraftPix](https://craftpix.net) - 2D, 3D, Ses, GUI, arka planlar, simgeler, döşeme setleri, oyun kitleri gibi Ücretsiz/Ücretli varlıklar.
  * [Freesound](https://freesound.org/) - Farklı CC lisanslarına sahip ücretsiz ortak ses kitaplığı teklifi.
  * [Oyun Simgeleri](https://game-icons.net/) - CC-BY lisansı altında sağlanan, ücretsiz stile sahip SVG/PNG simgeleri.
  * [GameDevMarket](https://gamedevmarket.net) - 2D, 3D, Ses, GUI gibi Ücretsiz/Ücretli varlıklar.
  * [Gamefresco.com](https://gamefresco.com/) - Her yerdeki oyun sanatçılarının ücretsiz oyun varlıklarını keşfedin, toplayın ve paylaşın.
  * [itch.io](https://itch.io/game-assets) - Spritelar, döşeme setleri ve karakter paketleri gibi Ücretsiz/Ücretli varlıklar.
  * [Kenney](https://www.kenney.nl/assets/) - Ücretsiz (CC0 1.0 Evrensel lisanslı) 2D, 3D, Ses ve kullanıcı arayüzü oyun varlıkları.
  * [LoSpec](https://lospec.com/) - Piksel sanatı ve diğer kısıtlayıcı dijital sanatlar oluşturmaya yönelik çevrimiçi araçlar, oyunlarınız için aralarından seçim yapabileceğiniz çok sayıda eğitim/palet listesi mevcuttur
  * [OpenGameArt](https://opengameart.org) - Müzik, sesler, hareketli görüntüler ve gifler gibi Açık Kaynak Oyun Varlıkları.
  * [Poliigon](https://www.poliigon.com/) - Ücretsiz ve ücretli dokular (değişken çözünürlükte), modeller, HDRI'ler ve fırçalar. Blender gibi yazılımlara aktarmak için ücretsiz eklentiler sunar.
  * [Poly Pizza](https://poly.pizza/) - Ücretsiz düşük poli 3D varlıklar

**[⬆️Başa Dön](#table-of-contents)**

## Other Free Resources

  * [360Converter](https://www.360converter.com/) - Dönüştürmek için ücretsiz katmanlı kullanışlı web sitesi: Videoyu Metne && Sesi Metne && Konuşmayı Metne && Gerçek Zamanlı Sesi Metne && YouTube Videosunu Metne && Video Altyazısı ekleyin. Belki kısa bir video dönüşümünde veya kısa bir youtube eğitiminde faydalı olabilir :)
  * [AdminMart](https://adminmart.com/) - Angular, Bootstrap, React, VueJs, NextJS ve NuxtJS ile oluşturulmuş Yüksek Kaliteli Ücretsiz ve Premium Yönetici Kontrol Paneli ve Web Sitesi Şablonları!
  * [Buttons Generator](https://markodenic.com/tools/buttons-generator/) - Projenizde kullanabileceğiniz 100'den fazla düğme.
  * [Framacloud](https://degooglisons-internet.org/en/) - Fransız kar amacı gütmeyen kuruluş [Framasoft](https://framasoft.org/en/) tarafından hazırlanan Ücretsiz/Libre Açık Kaynak Yazılım ve SaaS listesi.
  * [Ücretsiz Kod Araçları](https://freecodetools.org/) - %100 ücretsiz olan etkili kod araçları. Markdown düzenleyici, Kod küçültücü/güzelleştirici, QR kod oluşturucu, Açık Grafik Oluşturucu, Twitter kartı Oluşturucu ve daha fazlası.
  * [get.localhost.direct](https://get.localhost.direct) - Alt alan adı desteğiyle localhost geliştirme için daha iyi bir `*.localhost.direct` Wildcard genel CA imzalı SSL sertifikası
  * [GitHub Education](https://education.github.com/pack) - Öğrencilere yönelik ücretsiz hizmet koleksiyonu. Kayıt gerekli.
  * [Glob tester](https://globster.xyz/) - Glob modellerini tasarlamanıza ve test etmenize olanak tanıyan bir web sitesi. Ayrıca küresel kalıpları öğrenmek için kaynaklar sağlar.
  * [BT araçları](https://it-tools.tech/) - Geliştiriciler ve BT'de çalışan kişiler için faydalı araçlar.
  * [JSON Görüntüleyici Aracı](https://jsonviewertool.com/) - JSON verilerini doğrudan tarayıcıda görüntüleyin, biçimlendirin, doğrulayın, küçültün ve dönüştürün (API anahtarı gerekmez).
  * [Killer Coda](https://killercoda.com/) - Linux, Kubernetes, Konteynerler, Programlama, DevOps, Ağ İletişimi üzerinde çalışmak için tarayıcınızda etkileşimli oyun alanı
  * [Kody Tools](https://www.kodytools.com/dev-tools) - Biçimlendirici, küçültücü ve dönüştürücü dahil 100'den fazla geliştirme aracı.
  * [Markdown Araçları](https://markdowntools.com) - HTML, CSV'ler, PDF'ler, JSON ve Excel dosyalarını Markdown'a ve Markdown'dan dönüştürmek için araçlar
  * [Microsoft 365 Geliştirici Programı](https://developer.microsoft.com/microsoft-365/dev-program) - Microsoft 365 platformuna yönelik çözümler oluşturmak için ihtiyacınız olan ücretsiz bir sanal alan, araçlar ve diğer kaynakları edinin. Abonelik, yenilenebilir olan 90 günlük bir [Microsoft 365 E5 Aboneliği](https://www.microsoft.com/microsoft-365/enterprise/e5) (Windows hariç) şeklindedir. Geliştirme aşamasında aktifseniz yenilenir (telemetri verileri ve algoritmalar kullanılarak ölçülür).
  * [MySQL Visual Açıklama](https://mysqlexplain.com) - Yavaş sorguları optimize etmek için anlaşılması kolay ve ücretsiz MySQL EXPLAIN çıktı görselleştiricisi.
  * [PageTools](https://pagetools.co/) - Basit tek tıklamalı bir arayüzle temel web sitesi politikaları oluşturmanıza, sosyal medya biyografileri, gönderiler ve web sayfaları oluşturmanıza yardımcı olacak, sonsuza kadar ücretsiz yapay zeka destekli araçlardan oluşan bir paket sunar.
  * [Pyrexp](https://pythonium.net/regex) - Normal ifadelerde hata ayıklamak için ücretsiz web tabanlı normal ifade test aracı ve görselleştirici.
  * [Geliştiriciler için RedHat](https://developers.redhat.com) - Geliştiricilere özel olarak RHEL, OpenShift, CodeReady vb. dahil Red Hat ürünlerine ücretsiz erişim. Yalnızca bireysel plan. Referans için ücretsiz e-kitaplar da sunulmaktadır.
  * [regex101](https://regex101.com/) - Ücretsiz bu web sitesi normal ifadeleri (regex) test etmenize ve hata ayıklamanıza olanak tanır. Bir normal ifade düzenleyicisi ve test aracının yanı sıra normal ifadeyi öğrenmek için yararlı belgeler ve kaynaklar sağlar.
  * [sandbox.httpsms.com](https://sandbox.httpsms.com) - Test SMS mesajlarını ücretsiz olarak gönderin ve alın.
  * [SimpleBackups.com](https://simplebackups.com/) - Doğrudan bulut depolama sağlayıcılarında (AWS, DigitalOcean ve Backblaze) depolanan sunucular ve veritabanları (MySQL, PostgreSQL, MongoDB) için yedekleme otomasyon hizmeti. 1 yedekleme için ücretsiz bir plan sağlar.
  * [SimpleRestore](https://simplerestore.io) - Sorunsuz MySQL yedekleme geri yüklemesi. MySQL yedeklerini herhangi bir uzak veritabanına kod veya sunucu olmadan geri yükleyin.
  * [SnapShooter](https://snapshooter.com/) - DigitalOcean, AWS, LightSail, Hetzner ve Exoscale için doğrudan veritabanı, dosya sistemi ve s3 tabanlı depolamaya uygulama yedekleme desteğiyle yedekleme çözümü. Tek bir kaynak için günlük yedeklemeler içeren ücretsiz bir plan sağlar.
  * [Tablo Formatı Dönüştürücüsü](https://www.tableformatconverter.com) - Tablo verilerini CSV, HTML, JSON, Markdown ve daha fazlası gibi farklı formatlara dönüştürmek için ücretsiz bir araç.
  * [Tema seçimi](https://themeselection.com/) - Seçilmiş yüksek kaliteli, modern tasarımlı, profesyonel ve kullanımı kolay Ücretsiz Yönetici Kontrol Paneli Şablonu,
  * [ToolsHref](https://toolshref.com) - Java kodu oluşturma (JSON'dan POJO'ya, cURL'den Java'ya), statik analiz ve DevOps yapılandırma oluşturucularını (Docker, K8s, Nginx) içeren ücretsiz geliştirici yardımcı programlarından oluşan bir paket.
  * [Utils.fun](https://utils.fun/en) - Filigran oluşturma, ekran kaydetme, kodlama ve kod çözme, şifreleme ve şifre çözme ve kod biçimlendirme dahil olmak üzere tarayıcının bilgi işlem gücüne dayanan tüm çevrimdışı günlük ve geliştirme araçları tamamen ücretsizdir ve işlenmek üzere buluta herhangi bir veri yüklemez.
  * [Wikimint Geliştiricisi](https://developer.wikimint.com/p/tools.html) - Web geliştiricileri için CSS küçültme, küçültme, görüntü optimize edici, görüntü yeniden boyutlandırıcı, büyük/küçük harf dönüştürücü, CSS doğrulayıcı, JavaScript derleyici, HTML düzenleyici vb. içeren her zaman ücretsiz araçlar.
  * [WrapPixel](https://www.wrappixel.com/) - Angular, React, VueJs, NextJS ve NuxtJS ile oluşturulan Yüksek Kaliteli Ücretsiz ve Premium Yönetici kontrol paneli şablonunu indirin!
Uygulamalarınızı daha hızlı oluşturmak için HTML Temaları ve UI Kitleri!

**[⬆️Başa Dön](#table-of-contents)**
