# Yemək sifariş sistemi

## Proyekt haqqında

Bu proyektdə istifadəçilər yemək sifariş edə, öz sifarişlərinə nəzarət edə bilər və restoranlar da menyularını və sifarişlərini idarə edə, platforma üzərində olan satışlarına görə reportlar ala bilərlər. Proyektdə əsas üç rol var: İstifadəçi, Restoran və Admin. Və applikasiya hər rola uyğun davranış göstərə bilməlidir.

## Əsas özəllikləri

1. **Login/Register:**

   - İstifadəçilərin sistemə girişi çıxışı
   - Fərqli rollar(istifadəçi, Restoran və Admin)
     - İstifadəçi sadəcə əsas səhifədən yemək sifariş edə bilir
     - Restoran öz restoranını idarə edir xüsusi panel ilə, menyular əlavə edir və sair(ətraflı aşağıda)
     - Admin isə demək olar bütün sistem üzərində hakimiyyəti olur

2. **İstifadəçi özəllikləri:**

   - İlkin səhifədə olan ən məhşur yeməkləri görə bilir və onlardan istədiklərini sifariş verə bilir.
     > Ən məhşur yeməklər isə sifariş sayı müəyyən ədəddən(siz təyin edə bilərsiniz) çox olan ilk 10 yeməkdir
   - Restoranlar bölməsindən hansısa restoranı seçib onun yeməkləri ilə tanışa ola bilir və istəsə ordan sifariş edə bilir
   - Öz profilində özünə aid məlumatları dəyişə bilir
     > Bura vacibdir çünki sifariş verərkən default olaraq adresi onun qeydiyyat zamanı və ya sonra dəyişdiyi adres olur, təbii ki istəsə başqa adres seçə bilər
   - Orders bölməsinə keçərək verdiyi bütün sifarişləri detalları ilə görə bilir və istəsə bitmiş olan sifarişlərinin _Invoice_-ni(Çekini) görə bilir.
     > Invoice HTML kimi olmalıdı, ayrıca səhifə kimi verilib. İstəsəyə görə stilini dəyişmək olar.
   - MyCart bölməsi ilə də öz virtual arabasına əlavə elədiyi yeməkləri görə bilir istəsə çıxardır və ya sayını artıra bilir ən sonda isə checkout ilə sifarişini tamamlayır.

3. **Restoran özəllikləri:**

   - Restoranlar ilkin səhifədə öz statistikalarını görə bilir və istəsə pdf formatında report ala bilirlər(həm satdığı yeməklərin sayına görə həm də kateqoriyalara görə ki, beləcə hansı kateqoriyaya daha çox yatırım edəcəklərini görə bilsinlər)
   - Eləcə də özləri kateqoriyalar yarada bilir və bu kateqoriyaları idarə bilirlər. Lakin kateqoriya yaradan və silən zaman bunu yalnız admin qəbulu ilə edə bilirlər(əlavə challenge olsun🤠)
   - Kateqoriyalara əlavə olaraq restoranlar öz menyularını yarada və idarə edə bilirlər
   - Və təbii, olaraq ən vacibi öz sifarişlərini görə bilir və sifarişlərini idarə edə bilirlər, onların statuslarını dəyişə bilir və ya ümumiyyətlə silə bilirlər
     > Qeyd etmək lazımdır ki, restoran ui-ı ayrıca yoxdur sadəcə yazılan xüsusiyyətlər admin bölməsində mövcuddur, onlardan ehtiyac olan bölmələri kəsib istifadə etmək olar.
     > Və bir də ui tam olaraq ehtiyacları qarşılamaya bilər, burda sizə bir css biliklərini lazım ola bilər(növbəti challange🤠)
     > Məsələn əlavə olaraq hər restoranın ilkin səhifəsində onun profil şəklini görmək əla olar.

4. **Admin özəllikləri:**

   - Restoran üçün qeyd olunan bütün özəlliklər adminə də aiddir, sadəcə daha ümumi şəkli. Belə deyək ki, əgər restoran öz sifarişlərini görə bilirsə admin sistemdəki bütün sifarişləri görə bilir
   - Əlavə olaraq admin sistemdəki, istifadəçiləri və restoranları idarə bilir.
