
### 6. Answer the following questions clearly:

1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?

getElementById
শুধু ID দিয়ে খোঁজে
একটি মাত্র এলিমেন্ট রিটার্ন করে

getElementsByClassName
শুধু class name দিয়ে খোঁজে
একাধিক এলিমেন্টের একটি live collection রিটার্ন করে
DOM পরিবর্তন হলে এটি আপডেট হয়

querySelector
যেকোনো CSS সিলেক্টর দিয়ে খোঁজে (ID, class, tag সব)
প্রথম মিল পাওয়া একটি এলিমেন্ট রিটার্ন করে

querySelectorAll
যেকোনো CSS সিলেক্টর দিয়ে খোঁজে
সকল মিল পাওয়া এলিমেন্টের static NodeList রিটার্ন করে
DOM পরিবর্তন হলেও এটি আপডেট হয় না


2. How do you **create and insert a new element into the DOM**?
document.createElement() দিয়ে নতুন এলিমেন্ট তৈরি করতে হয়।

সেই এলিমেন্টে কনটেন্ট বা অ্যাট্রিবিউট যোগ করতে হয়।

তারপর appendChild(), prepend() বা insertBefore() ব্যবহার করে সেটিকে DOM-এর কোনো প্যারেন্ট এলিমেন্টে যুক্ত করতে হয়।

3. What is **Event Bubbling** and how does it work?

যখন কোনো child element-এ ইভেন্ট (যেমন: click) ঘটে, তখন:
প্রথমে সেই child element-এ ইভেন্টটি ঘটে
এরপর সেটি তার parent element-এ যায়


4. What is **Event Delegation** in JavaScript? Why is it useful?

Event Delegation হলো এমন একটি টেকনিক, যেখানে কোনো parent element-এ ইভেন্ট listener বসিয়ে, child element-এ হওয়া ইভেন্ট হ্যান্ডেল করা হয়।
এতে child গুলোর জন্য আলাদাভাবে ইভেন্ট listener বসাতে হয় না।


5. What is the difference between **preventDefault() and stopPropagation()** methods?

preventDefault()
এটি ব্রাউজারের ডিফল্ট আচরণ বন্ধ করে দেয়
ইভেন্ট বাবলিং বন্ধ করে না


stopPropagation()
ইভেন্টটি parent element-এ propagate (বাবল) হওয়া বন্ধ করে
কিন্তু ডিফল্ট অ্যাকশন চালু থাকে




