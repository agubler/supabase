<p align="center">
<img width="300" src="https://raw.githubusercontent.com/supabase/supabase/master/packages/common/assets/images/supabase-logo-wordmark--light.svg#gh-light-mode-only">
<img width="300" src="https://raw.githubusercontent.com/supabase/supabase/master/packages/common/assets/images/supabase-logo-wordmark--dark.svg#gh-dark-mode-only">
</p>

---

# Supabase

[Supabase](https://supabase.com) একটি ওপেন সোর্স ফায়ারবেস বিকল্প। আমরা এন্টারপ্রাইজ-গ্রেড ওপেন সোর্স টুল ব্যবহার করে Firebase-এর বৈশিষ্ট্য তৈরি করছি।

- [x] হোস্ট করা পোস্টগ্রেস ডাটাবেস
- [x] রিয়েলটাইম সদস্যতা
- [x] প্রমাণীকরণ এবং অনুমোদন
- [x] স্বয়ংক্রিয়ভাবে তৈরি APIs
- [x] ড্যাশবোর্ড
- [x] স্টোরেজ
- [x] ফাংশন

![Supabase Dashboard](https://raw.githubusercontent.com/supabase/supabase/master/apps/www/public/images/github/supabase-dashboard.png)

## ডকুমেন্টেশন

সম্পূর্ণ ডকুমেন্টেশনের জন্য, দেখুন [supabase.com/docs](https://supabase.com/docs)

কিভাবে অবদান রাখতে হয় তা দেখতে, পরিদর্শন করুন [Getting Started](../DEVELOPERS.md)

## কমিউনিটি ও সাপোর্ট

- [কমিউনিটি ফোরাম](https://github.com/supabase/supabase/discussions). এর জন্য সর্বোত্তম: তৈরিতে সহায়তা, ডাটাবেস সেরা অনুশীলন সম্পর্কে আলোচনা।
- [গিঠাব ইস্যু](https://github.com/supabase/supabase/issues). এর জন্য সেরা: সুপাবেস ব্যবহার করে আপনি যে বাগ এবং ত্রুটির সম্মুখীন হন।
- [ইমেইল সাপোর্ট](https://supabase.com/docs/support#business-support). এর জন্য সেরা: আপনার ডাটাবেস বা অবকাঠামো নিয়ে সমস্যা।
- [ডিসকোর্ড](https://discord.supabase.com). এর জন্য সর্বোত্তম: আপনার অ্যাপ্লিকেশনগুলি ভাগ করা এবং সম্প্রদায়ের সাথে হ্যাঙ্গআউট করা৷

## স্ট্যাটাস

- [x] আলফা: আমরা গ্রাহকদের একটি বন্ধ সেটের সাথে সুপাবেস পরীক্ষা করছি
- [x] পাবলিক আলফা: যে কেউ [app.supabase.com](https://app.supabase.com) এ সাইন আপ করতে পারেন। কিন্তু আমাদের উপর সহজ যান, কয়েক kinks আছে
- [x] পাবলিক বিটা: বেশিরভাগ নন-এন্টারপ্রাইজ ব্যবহারের ক্ষেত্রে যথেষ্ট স্থিতিশীল
- [ ] পাবলিক: উত্পাদন প্রস্তুত

আমরা বর্তমানে পাবলিক বিটাতে আছি। বড় আপডেটের বিজ্ঞপ্তি পেতে এই রেপোর "রিলিজ" দেখুন।

<kbd><img src="https://raw.githubusercontent.com/supabase/supabase/d5f7f413ab356dc1a92075cb3cee4e40a957d5b1/web/static/watch-repo.gif" alt="এই রেপো দেখুন"/></kbd>

---

## কিভাবে এটা কাজ করে

সুপাবেস হল ওপেন সোর্স টুলের সংমিশ্রণ। আমরা এন্টারপ্রাইজ-গ্রেড, ওপেন সোর্স পণ্য ব্যবহার করে Firebase-এর বৈশিষ্ট্য তৈরি করছি। যদি MIT, Apache 2, বা সমতুল্য ওপেন লাইসেন্স সহ টুল এবং সম্প্রদায়গুলি বিদ্যমান থাকে, আমরা সেই টুলটি ব্যবহার করব এবং সমর্থন করব। যদি টুলটি বিদ্যমান না থাকে, তাহলে আমরা নিজেরাই এটি তৈরি এবং ওপেন সোর্স করি। সুপাবেস ফায়ারবেসের 1-থেকে-1 ম্যাপিং নয়। ওপেন সোর্স টুল ব্যবহার করে ডেভেলপারদের ফায়ারবেসের মতো ডেভেলপার অভিজ্ঞতা দেওয়াই আমাদের লক্ষ্য।

**স্থাপত্য**

সুপাবেস হল একটি [হোস্ট করা প্ল্যাটফর্ম](https://app.supabase.com)। আপনি সাইন আপ করতে পারেন এবং কিছু ইনস্টল না করে সুপাবেস ব্যবহার শুরু করতে পারেন।
এছাড়াও আপনি [স্ব-হোস্ট](https://supabase.com/docs/guides/hosting/overview) এবং [স্থানীয়ভাবে বিকাশ](https://supabase.com/docs/guides/local-development) করতে পারেন।

![আর্কিটেকচার](https://user-images.githubusercontent.com/70828596/187547862-ffa9d058-0c3a-4851-a3e7-92ccfca4b596.png)

- [PostgreSQL](https://www.postgresql.org/) হল একটি অবজেক্ট-রিলেশনাল ডাটাবেস সিস্টেম যার 30 বছরের বেশি সক্রিয় বিকাশ রয়েছে যা এটিকে নির্ভরযোগ্যতা, বৈশিষ্ট্যের দৃঢ়তা এবং কর্মক্ষমতার জন্য একটি শক্তিশালী খ্যাতি অর্জন করেছে।
- [রিয়েলটাইম](https://github.com/supabase/realtime) হল একটি Elixir সার্ভার যা আপনাকে ওয়েবসকেট ব্যবহার করে PostgreSQL সন্নিবেশ, আপডেট এবং মুছে ফেলা শুনতে দেয়। ডাটাবেস পরিবর্তনের জন্য রিয়েলটাইম পোল পোস্টগ্রেসের অন্তর্নির্মিত প্রতিলিপি কার্যকারিতা, পরিবর্তনগুলিকে JSON-এ রূপান্তরিত করে, তারপর অনুমোদিত ক্লায়েন্টদের কাছে ওয়েবসকেটের মাধ্যমে JSON সম্প্রচার করে।
- [PostgREST](http://postgrest.org/) একটি ওয়েব সার্ভার যা আপনার PostgreSQL ডাটাবেসকে সরাসরি একটি RESTful API-তে পরিণত করে
- [স্টোরেজ](https://github.com/supabase/storage-api) অনুমতিগুলি পরিচালনা করতে Postgres ব্যবহার করে S3-এ সঞ্চিত ফাইলগুলি পরিচালনা করার জন্য একটি RESTful ইন্টারফেস প্রদান করে।
- [postgres-meta](https://github.com/supabase/postgres-meta) হল আপনার পোস্টগ্রেস পরিচালনা করার জন্য একটি RESTful API, যা আপনাকে টেবিল আনতে, ভূমিকা যোগ করতে এবং কোয়েরি চালানোর অনুমতি দেয়।
- [GoTrue](https://github.com/netlify/gotrue) ব্যবহারকারীদের পরিচালনা এবং SWT টোকেন ইস্যু করার জন্য একটি SWT ভিত্তিক API।
- [কং](https://github.com/Kong/kong) হল একটি ক্লাউড-নেটিভ API গেটওয়ে।

#### ক্লায়েন্ট লাইব্রেরি

ক্লায়েন্ট লাইব্রেরির জন্য আমাদের পদ্ধতি মডুলার। প্রতিটি উপ-লাইব্রেরি একটি একক বহিরাগত সিস্টেমের জন্য একটি স্বতন্ত্র বাস্তবায়ন। এটি এমন একটি উপায় যা আমরা বিদ্যমান সরঞ্জামগুলিকে সমর্থন করি৷

<table style="table-layout:fixed; white-space: nowrap;">৷
  <tr>
    <th>ভাষা</th>
    <th>ক্লায়েন্ট</th>
    <th colspan="4">ফিচার-ক্লায়েন্ট (সুপাবেস ক্লায়েন্টে বান্ডিল)</th>
  </tr>
  <tr>
    <th></th>
    <th>Supabase</th>
    <th><a href="https://github.com/postgrest/postgrest" target="_blank" rel="noopener noreferrer">PostgREST</a></th>
    <th><a href="https://github.com/supabase/gotrue" target="_blank" rel="noopener noreferrer">GoTrue</a></th>
    <th><a href="https://github.com/supabase/realtime" target="_blank" rel="noopener noreferrer">রিয়েলটাইম</a></th>
    <th><a href="https://github.com/supabase/storage-api" target="_blank" rel="noopener noreferrer">স্টোরেজ</a></th>
  </tr>
  <!-- নতুন সারির জন্য টেমপ্লেট -->
  <!-- সারি শুরু করুন
  <tr>
    <td>lang</td>
    <td><a href="https://github.com/supabase-community/supabase-lang" target="_blank" rel="noopener noreferrer">supabase-lang</a></td>
    <td><a href="https://github.com/supabase-community/postgrest-lang" target="_blank" rel="noopener noreferrer">postgrest-lang</a></td>
    <td><a href="https://github.com/supabase-community/gotrue-lang" target="_blank" rel="noopener noreferrer">gotrue-lang</a></td>
    <td><a href="https://github.com/supabase-community/realtime-lang" target="_blank" rel="noopener noreferrer">রিয়েলটাইম-ল্যাং</a></td>
    <td><a href="https://github.com/supabase-community/storage-lang" target="_blank" rel="noopener noreferrer">স্টোরেজ-ল্যাং</a></td>
  </tr>
  শেষ সারি -->
  <th colspan="6">⚡️ অফিসিয়াল ⚡️</th>
  <tr>
    <td>জাভাস্ক্রিপ্ট (টাইপস্ক্রিপ্ট)</td>
    <td><a href="https://github.com/supabase/supabase-js" target="_blank" rel="noopener noreferrer">supabase-js</a></td>
    <td><a href="https://github.com/supabase/postgrest-js" target="_blank" rel="noopener noreferrer">postgrest-js</a></td>
    <td><a href="https://github.com/supabase/gotrue-js" target="_blank" rel="noopener noreferrer">gotrue-js</a></td>
    <td><a href="https://github.com/supabase/realtime-js" target="_blank" rel="noopener noreferrer">রিয়েলটাইম-জেএস</a></td>
    <td><a href="https://github.com/supabase/storage-js" target="_blank" rel="noopener noreferrer">storage-js</a></td>
  </tr>
  <th colspan="6">💚 সম্প্রদায় 💚</th>
  <tr>
    <td>C#</td>
    <td><a href="https://github.com/supabase-community/supabase-csharp" target="_blank" rel="noopener noreferrer">supabase-csharp</a></td>
    <td><a href="https://github.com/supabase-community/postgrest-csharp" target="_blank" rel="noopener noreferrer">postgrest-csharp</a></td>
    <td><a href="https://github.com/supabase-community/gotrue-csharp" target="_blank" rel="noopener noreferrer">gotrue-csharp</a></td>
    <td><a href="https://github.com/supabase-community/realtime-csharp" target="_blank" rel="noopener noreferrer">রিয়েলটাইম-csharp</a></td>
    <td>-</td>
  </tr>
  <tr>
    <td>ডার্ট (ফ্লাটার)</td>
    <td><a href="https://github.com/supabase/supabase-dart" target="_blank" rel="noopener noreferrer">supabase-dart</a></td>
    <td><a href="https://github.com/supabase/postgrest-dart" target="_blank" rel="noopener noreferrer">postgrest-dart</a></td>
    <td><a href="https://github.com/supabase/gotrue-dart" target="_blank" rel="noopener noreferrer">gotrue-dart</a></td>
    <td><a href="https://github.com/supabase/realtime-dart" target="_blank" rel="noopener noreferrer">রিয়েলটাইম-ডার্ট</a></td>
    <td><a href="https://github.com/supabase/storage-dart" target="_blank" rel="noopener noreferrer">storage-dart</a></td>
  </tr>
  <tr>
    <td>গো</td>
    <td>-</td>
    <td><a href="https://github.com/supabase-community/postgrest-go" target="_blank" rel="noopener noreferrer">postgrest-go</a></td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>জাভা</td>
    <td>-</td>
    <td>-</td>
    <td><a href="https://github.com/supabase-community/gotrue-java" target="_blank" rel="noopener noreferrer">gotrue-java</a></td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>কোটলিন</td>
    <td>-</td>
    <td><a href="https://github.com/supabase-community/postgrest-kt" target="_blank" rel="noopener noreferrer">postgrest-kt</a></td>
    <td><a href="https://github.com/supabase-community/gotrue-kt" target="_blank" rel="noopener noreferrer">gotrue-kt</a></td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>পাইথন</td>
    <td><a href="https://github.com/supabase-community/supabase-py" target="_blank" rel="noopener noreferrer">supabase-py</a></td>
    <td><a href="https://github.com/supabase-community/postgrest-py" target="_blank" rel="noopener noreferrer">postgrest-py</a></td>
    <td><a href="https://github.com/supabase-community/gotrue-py" target="_blank" rel="noopener noreferrer">gotrue-py</a></td>
    <td><a href="https://github.com/supabase-community/realtime-py" target="_blank" rel="noopener noreferrer">realtime-py</a></td>
    <td>-</td>
  </tr>
  <tr>
    <td>রুবি</td>
    <td><a href="https://github.com/supabase-community/supabase-rb" target="_blank" rel="noopener noreferrer">supabase-rb</a></td>
    <td><a href="https://github.com/supabase-community/postgrest-rb" target="_blank" rel="noopener noreferrer">postgrest-rb</a></td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>রাস্ট</td>
    <td>-</td>
    <td><a href="https://github.com/supabase-community/postgrest-rs" target="_blank" rel="noopener noreferrer">postgrest-rs</a></td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>সুইফট</td>
    <td><a href="https://github.com/supabase-community/supabase-swift" target="_blank" rel="noopener noreferrer">supabase-swift</a></td>
    <td><a href="https://github.com/supabase-community/postgrest-swift" target="_blank" rel="noopener noreferrer">postgrest-swift</a></td>
    <td><a href="https://github.com/supabase-community/gotrue-swift" target="_blank" rel="noopener noreferrer">gotrue-swift</a></td>
    <td><a href="https://github.com/supabase-community/realtime-swift" target="_blank" rel="noopener noreferrer">রিয়েলটাইম-সুইফট</a></td>
    <td><a href="https://github.com/supabase-community/storage-swift" target="_blank" rel="noopener noreferrer">স্টোরেজ-সুইফট</a></td>
  </tr>
</table>

## অনুবাদ

- [অনুবাদের তালিকা](/i18n/languages.md) <!--- Keep only this -->

## স্পনসর

[![নতুন স্পনসর](https://user-images.githubusercontent.com/10214025/90518111-e74bbb00-e198-11ea-8f88-c9e3c1aa4b5b.png)](https://github.com/sponsors/supabase)
