Activity Center Demo APK project

এটি Telegram-এর বাইরে চলা একটি স্বতন্ত্র Android demo app। এতে তারিখ বাছাই, ডেমো history card, preview dialog ও নিচের navigation bar-এর visual sample আছে। Telegram account/message data এতে যুক্ত নয়; Go বাটন আসল Telegram chat খুলবে না।

ফোন থেকে APK বানানোর সহজ পদ্ধতি:
1) ZIP-টি GitHub-এ নতুন repository হিসেবে upload করুন (সব ফাইল ও .github/workflows/build.yml সহ)।
2) GitHub repository > Actions > “Build Activity Center APK” > Run workflow চাপুন।
3) কাজ শেষ হলে workflow run-এর Artifacts থেকে ActivityCenter-debug-apk.zip নামান।
4) ZIP extract করে app-debug.apk ইনস্টল করুন। নিজের তৈরি APK হওয়ায় Android install confirmation আসতে পারে।

Build environment: Java 17, Gradle 8.9, Android SDK platform 35.

এটি Telegram-এর অফিসিয়াল অ্যাপ নয় এবং Telegram source code-এ কোনো পরিবর্তন করে না। Telegram-এ ফিচার যুক্ত করতে আলাদা source integration, real MessagesStorage/MessagesController wiring, navigation integration, tests এবং upstream review দরকার।
