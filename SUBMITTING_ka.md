# როგორ გავაგზავნოთ — Pull Request-ით

ეს არასდროს გაგიკეთებიათ და არაუშავს — ყველა ნაბიჯი აქ არის. **Fork**
არის ამ რეპოზიტორის თქვენი საკუთარი ასლი GitHub-ზე. **Branch** არის
ადგილი, სადაც თქვენი ცვლილებები ინახება. **Pull Request (PR)** სთხოვს
თქვენი branch-ის ცვლილებების შერწყმას ორიგინალ რეპოზიტორთან.

## 1. დააინსტალირეთ Git

- **Windows:** დააინსტალირეთ [Git for Windows](https://git-scm.com/download/win). გამოიყენეთ "Git Bash" ტერმინალად შემდეგი ნაბიჯებისთვის.
- **macOS:** გახსენით Terminal და გაუშვით `git --version`.
- **Linux:** `sudo apt install git` (Debian/Ubuntu).

დარწმუნდით რომ იმუშავა:
```
git --version
```

## 2. შექმენით GitHub ანგარიში

თუ არ გაქვთ, დარეგისტრირდით [github.com](https://github.com)-ზე.

## 3. დააკონფიგურირეთ Git თქვენი სახელით და ელფოსტით

```
git config --global user.name "თქვენი სახელი"
git config --global user.email "you@example.com"
```

## 4. Fork-ი გაუკეთეთ ამ რეპოზიტორს

გადადით ამ რეპოზიტორის GitHub გვერდზე და დააჭირეთ **Fork**-ს
(ზედა მარჯვენა კუთხეში).

## 5. Clone გაუკეთეთ თქვენს fork-ს

```
git clone https://github.com/<თქვენი-username>/python-127-homework-1.git
cd python-127-homework-1
```

## 6. შექმენით branch თქვენი GitHub username-ის სახელით

```
git checkout -b <თქვენი-username>
```

## 7. შექმენით თქვენი საქაღალდე და დაამატეთ ფაილები

`submissions/`-ის შიგნით შექმენით საქაღალდე თქვენი username-ით.

**მხოლოდ თქვენი საკუთარი საქაღალდე.** არ შეცვალოთ `README.md`,
`EXERCISES.md`, `SUBMITTING.md`, ან სხვა სტუდენტის საქაღალდე.

## 8. გაუშვით ყველა ფაილი commit-მდე

```
python submissions/<თქვენი-username>/exercise_1.py
```

## 9. Commit და push გაუკეთეთ თქვენს branch-ს

```
git add .
git commit -m "Add homework 1"
git push -u origin <თქვენი-username>
```

## 10. გახსენით Pull Request

**სათაური:** `Homework 1 - თქვენი სახელი`.

## 11. დაელოდეთ განხილვას

ვერ დააგზავნით პირდაპირ ორიგინალ რეპოზიტორში — მისი `main` branch
დაცულია. ინსტრუქტორი ავტომატურად ემატება როგორც reviewer.
