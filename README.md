# Akademik Hedef Takipçisi

Akademik Hedef Takipçisi, öğrencilerin dönemlik akademik hedeflerini belirleyip takip edebileceği bir Android uygulamasıdır. Kullanıcılar derslerini ekleyebilir, notlarını takip edebilir ve mevcut GPA ile hedef GPA'yı karşılaştırabilir.

## Özellikler

* Kullanıcı kayıt ve giriş sistemi (Firebase Authentication)
* Ders ekleme ve silme
* GPA hesaplama
* Hedef GPA belirleme
* Mevcut GPA ve hedef GPA karşılaştırması
* Ders listesini görüntüleme
* Transkript PDF oluşturma
* Modern Android arayüzü (Jetpack Compose)

## Kullanılan Teknolojiler

**Frontend**

* Kotlin
* Jetpack Compose
* Android Studio
* MVVM Architecture

**Backend**

* Firebase Authentication
* Firebase Firestore

**Libraries**

* Navigation Compose
* Kotlin Coroutines
* Firebase SDK

## Proje Yapısı

```
AkademikHedefTakipcisi

app
 ├── ui
 │   ├── screens
 │   │   ├── LoginScreen.kt
 │   │   ├── RegisterScreen.kt
 │   │   ├── DashboardScreen.kt
 │   │   └── AddCourseScreen.kt
 │   │
 │   ├── components
 │   │   ├── CourseCard.kt
 │   │   └── ProgressChart.kt
 │   │
 │   └── theme
 │
 ├── models
 │   ├── Course.kt
 │   └── User.kt
 │
 ├── repository
 │   └── FirebaseRepository.kt
 │
 ├── viewmodel
 │   ├── DashboardViewModel.kt
 │   └── CourseViewModel.kt
 │
 ├── navigation
 │   └── NavigationGraph.kt
 │
 └── utils
     ├── GPACalculator.kt
     └── PdfGenerator.kt
```

## GPA Hesaplama

```
GPA = Σ(grade × credit) / Σ(credit)
```

## Uygulama Akışı

```
Login
   ↓
Register
   ↓
Dashboard
   ↓
Add Course
   ↓
Back to Dashboard
```

## Kurulum

1. Bu repository'i klonlayın:

```
git clone https://github.com/mohamedalimohamed1/AkademikHedefTakipcisi.git
```

2. Android Studio ile projeyi açın.

3. Firebase projesi oluşturun.

4. `google-services.json` dosyasını `app/` klasörüne ekleyin.

5. Uygulamayı çalıştırın.

## Gelecek Geliştirmeler

* Grafiksel GPA analizi
* Ders düzenleme
* Dark mode
* Bildirim sistemi
* Akademik ilerleme raporları

## Geliştirici

Mohamed Ali Mohamed
Computer Engineering Student
