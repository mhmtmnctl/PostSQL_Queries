/*
-- GROUP BY -- HAVİNG --
HAVING ifadesinin işlevi WHERE ifadesininkine çok benziyor. Ancak kümeleme fonksiyonları ile
WHERE ifadesi birlikte kullanılmadığında HAVING ifadesine ihtiyac duyulmuştur
GROUP BY ile kullanılır gruplamadan sonraki şart için group by dan sonra HAVING kullanılır

*/

--Maaş ortalaması 3000’den fazla olan ülkelerdeki erkek çalışanların maaş ortalaması.
SELECT ulke, round(avg(maas)) as maas_ortalamasi from personel
WHERE cinsiyet='E'
group by ulke 
having avg(maas)>3000

--Erkek çalışanların sayısı 1’den fazla olan ülkelerin maaş ortalamasını getiren sorgu
select ulke, avg(maas) from personel WHERE cinsiyet='E' group by ulke having count(*)>1