# hangfire-webapi
Hangfire background'da işləyəcək işlərimizi idarə etməyə imkan verən open source library'dır. Daxili olaraq təmin etdiyi idarə paneli ilə biz vaxtı çatmamış işi işə sala, dayandıra və qısa müddətə idarə edə bilərik. Məsələn, hər gün saat 04:00-da log'lari silmək istəyə bilərik.

FireAndForgot
Bir gedişdə (1 dəfə) işləyəcək davamlı olmayan kodunuz varsa istifadə edə biləcəyiniz növdür. Məsələn, saytınızda qeydiyyatdan keçmiş istifadəçilərə e-poçt göndərmək.
Delayed
Müəyyən bir müddətdən sonra işləməli olan işlər üçün istifadə olunan növdür. Məsələn, istifadəçi saytınızda alış-veriş etdikdən 30 dəqiqə sonra e-poçt vasitəsilə başqa məhsul təklif etmək istəyə bilərsiniz. FireAndForgot tipindən yeganə fərq odur ki, o, müəyyən edildiyi andan müəyyən vaxtdan sonra (məsələn, 30 dəqiqədən sonra, 1 həftədən sonra) işləməlidir.
Recurring
Müəyyən fasilələrlə işləməyi tələb edən işlər üçün istifadə olunan növdür. Məsələn, hər ayın 1-də hesabat yaratmaq istədiyiniz işiniz varsa.
Təkrarlanan iş növünü təyin edərkən cron ifadə xüsusiyyətinə ehtiyacımız ola bilər. CronExpression xüsusi olaraq unix və ya linux əməliyyat sistemləri üçün müəyyən vaxt intervalında və arxa fonda istənilən tapşırıqları yerinə yetirmək üçün istifadə olunan bir vasitədir. Bu alətlə biz vaxtı təyin edə bilərik. Cron dəyəri yaratmaq üçün nümunə sayt: https://crontab.guru/

Continuations
Yaratdığınız digər işlərdən sonra işləyəcək işlər üçün istifadə olunan növdür. Bir sözlə, işdən sonra işləməkdir. Bu iş müvafiq iş tərifi ID ilə proses tamamlandıqdan sonra işləyəcək.

Batch ve Batch Continuations (pullu)
Bu, toplu emal həyata keçirərkən istifadə edəcəyiniz iş növüdür. Məsələn, 500 iş görəcəksinizsə, for döngəsi ilə geri dönərkən xəta ala bilərsiniz. Bu iş növü ilə biz asanlıqla idarə edə və səhvləri tuta bilərik. Başqa sözlə, qısa qruplarda görülən iş növüdür. Bulk Tracks qrup hərəkətlərindən sonra görüləcək işlər üçündür.
