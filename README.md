# End-striyel-Elektronik-ve-Robotik-Gelistirme-ve-Uyum-Dersi-2- DEV C++
## 	//Aritmetik operatörler  Kodları
  <img width="1792" height="995" alt="image" src="https://github.com/user-attachments/assets/0324af41-16da-4178-8728-631b330f7efe" />
**    #include <iostream>
      
      using namespace std;
      
      int main(int argc, char** argv) {
      	
      	cout<<25+36<<endl;
	   
      	cout<<65-250<<endl;
      	
      	
	
}
  <img width="1011" height="743" alt="image" src="https://github.com/user-attachments/assets/25787f9b-0a8b-400b-9233-02b733cb3207" />

**  #include <iostream>

using namespace std;

int main(int argc, char** argv) {
	//Aritmetik operatörler 
	//+ -> Toplama 
	// --> Çıkarma
	//  * ->Çarpma
	//  /  -> Bölme
	// % -> Mod alma
	cout<<25+36<<endl;
	cout<<65-250<<endl;
	cout<<65*85<<endl;
	cout<<65/5<<endl;
	cout<<140%7<<endl;
	
	
	
}

**    //string veri
	string ad = "queen" ;
	string soyad = "software";
	
	 string metin = ad + soyad ;
	 cout<<metin<<endl; 

  -çıktı olarak queensoftware gelecek
  <img width="813" height="1028" alt="image" src="https://github.com/user-attachments/assets/3df0f37d-5053-4c2a-9546-47748f6975aa" />

	
##	//Mantıksal Operatorler
	//  || Or(veya)
	// &&  AND (Ve) 
	
  

***
	
	//Mantıksal Operatorler
	//  || Or(veya)
	// &&  AND (Ve) 
	
	cout <<"Mantiksal Operatorler"<<endl;
	
	   
	 bool a1 =  (25 <35) && (45 ==45);
	 //          1        ve     1    =1 
	 
	bool a2 = 45 <25 || 35 >96;
	//           0  veya  0 = 0
	
	bool a3 = 74 >= 75 || 45>=-54;	
	 //        0       veya  1 = 1      
	 
	cout<<a1<<endl;
	cout<<a2<<endl;
	cout<<a3<<endl;
 <img width="1913" height="1017" alt="image" src="https://github.com/user-attachments/assets/a1fe5fe5-5da0-404e-a68d-bf8ca8cca568" />

	
	   

## Ternary operatörü

	//Ternary operatörü  ? , :
	
	int age;
	cout<<"Lutfen yas bilginizi giriniz."<<endl;
	cin>>age;
	
	string message =(age>=18) ?  "Resitsiniz." : "Resit Degilsiniz";
	cout<<message<<endl;


<img width="1189" height="835" alt="image" src="https://github.com/user-attachments/assets/a67efd85-ad87-4004-981f-ec397da7c64f" />


## Artırma azaltma operatörleri	
	
	//Artırma azaltma operatörleri
	// ++ veya -- operatörleri kullanarak işlemler uygulanır.
	cout<<"Arttirma ve azaltma operatörleri "<<endl;
	int X =10;
	X++ ; //Önce değeri kullan sonra arttır .
	++X;  // İlk önce değeri arttır sonra değeri kullan
	cout<<X<<endl;	
	
	
	int y = 10;
	cout<<"++y  :"<<++y<<endl;  //11 
	cout<<"y++: "<<y++<<endl;  //11 
	cout<<"y : "<<y<<endl; //12
	
	int z = 14;
	
		cout<<"--z  :"<<--z<<endl;  //13
	cout<<"z--: "<<z--<<endl;  //13 
	cout<<"z : "<<z<<endl; //12
	
	int r = z+=5;
	cout<<r<<endl;
	
	int x1 = z*=3;
	 r = r *3; 
	// 17 = 17 * 3
	 
	cout<<r<<endl;
		
		int a9 =  10;
	a9 = a9 *6;
	//a9 =10(eksi)
	cout<<a9<<endl;


## Örnek bir proje yapımı :
### Kullanıcıdan ders dı ve 3 tane ders notu alınıp ortalamasının hesaplanması


#include <iostream>

using namespace std;

int main(int argc, char** argv) {
	
	//Kullanıcıdan ders adı ve 3 not bilgisini aldıktan sonra 
	//ekran çıktısı olarak  Ders Adı : ,Not Ortolaması:
	
	string lesson;
	double not1 ,not2 ,not3;
	cout<<"Lutfen Ders adini giriniz . "<<endl;
	cin>> lesson;
	
	cout<<"Lutfen 1.ders notunu giriniz : "<<endl;
	cin>>not1;
	
		cout<<"Lutfen 2.ders notunu giriniz : "<<endl;
	cin>>not2;
	
		cout<<"Lutfen 3.ders notunu giriniz : "<<endl;
	cin>>not3;
	
	
	double toplam = not1 + not2+ not3;
	double ortalama = toplam /3;
	
	cout<<"Dersin adi : "<<lesson<<" Ortalamasi : "<<ortalama<<endl;
}



<img width="1798" height="894" alt="image" src="https://github.com/user-attachments/assets/e05ab3a9-a3ac-4c79-b1ad-c82c4d0a4793" />


### Vücut kitle endeksi hesaplama :

	//AD ,soyad,kilo  ,boy    vki = kilo(kg) / boy*boy (m)
	int main(int argc, char** argv) {


 	string ad;
    string soyad;
    double kilo ;
    double boy;
    
    cout<<"Lutfen adinizi giriniz "<<endl;
    cin>> ad;
    
	cout<<"Lutfen soyad giriniz "<<endl;
    cin>> soyad;
    
    cout<<"Lutfen kilo giriniz "<<endl;
    cin>> kilo;
    
     cout<<"Lutfen boy giriniz "<<endl;
    cin>> boy;
    
    
    
    
    
     double vki = kilo / (boy * boy);

    cout<< "\n--- Sonuc ---" <<endl;
    cout<< "Ad Soyad: " << ad << " " << soyad <<endl;
    cout<< "Vucut Kitle Endeksiniz: " << vki <<endl;

    if (vki < 18.5) {
        cout << "Durum: Zayif"<<endl;
    } else if (vki >= 18.5 && vki < 24.9) {
       cout << "Durum: Normal" << endl;
    } else if (vki >= 24.9 && vki < 29.9) {
      cout << "Durum: Kilolu" <<endl;
    } else {
    cout << "Durum: Obez" <<endl;
    }

    return 0;
    
<img width="1594" height="935" alt="image" src="https://github.com/user-attachments/assets/9f0b514e-e864-4f24-97f1-3a368c99868e" />


## Karar mekanizmaları

### Ehliyet alınabilir mi projesi:
  // Eğer yaş 18 den büyükse ve bütççe 500k dan fazlaise ehliyet alınabilir.Aksi taktirde ehliyet alınamaz.
  
	  int age = 19;
	  int budget =5000000;
	  if (age  >=18 && budget>500000){
	  	cout<<"Ehliyet alabilirsiniz."<<endl;
	  }else{
	  		cout<<"Ehliyet alamazsiniz."<<endl;
	  }



### Sayı pozitif mi? negatif mi ? 0 mı?
		int  number = -65;
   
	   if (number > 0){
	   		cout<<"Sayi pozitiftir."<<endl;
	   }
	   else if (number ==0 ){
	   	cout<<"Sayi 0dir."<<endl;
	   	
	   }else{
	   	cout<<"sayi negatiftir."<<endl;
	   }
###  Tek çift sayı bulma

	  // number sayısı tek mi çift mi bulalım
  
     int  number = 66;
     
  	if (number % 2 ==0) {
  	cout<<"cift";

	  }else{
	  	cout<<"tek";
	  }
  
  
  












































