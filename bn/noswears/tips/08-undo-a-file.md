---
tags: tip
title: ওহ গিট, আমার কোনও ফাইলের পরিবর্তনগুলি পূর্বাবস্থায় ফিরিয়ে আনা দরকার!
id: undo-a-file
order: 8
---

```git
# ফাইলটি পরিবর্তিত হওয়ার আগের একটি কমিটের হ্যাশ সন্ধান করুন
git log
# লগ হিস্টরির উপরে এবং নীচে স্ক্রোল করতে অ্যারো কী-গুলি ব্যবহার করুন
# আপনার কমিটটা একবার পেয়ে গেলে হ্যাশটি সংরক্ষণ করুন
git checkout [saved hash] -- path/to/file
# ফাইলটির পুরাতন ভার্সনটা আপনার ইনডেক্স এ থাকবে
git commit -m "Wow, you don't have to copy-paste to undo"
```

অবশেষে যখন আমি এটি বুঝতে পারলাম এটি ছিল বিশাল। বিশাল. বিশাল. তবে চিন্তা করুন, কোন গ্রহে `checkout --` কে, কোন ফাইলকে পূর্বাবস্থায় ফিরিয়ে আনার সেরা উপায় হিসাবে দেখবে?
