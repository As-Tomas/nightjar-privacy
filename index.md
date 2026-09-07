# Nightjar — Privacy Policy

**Version 1.0 · 2026-09-06 · Nightjar for Android (`io.nightjar.app`)**

## The one-minute version

- Your dreams stay on your phone. We never see them. There is no account and no server
  to send them to.
- The journal is stored in an encrypted database. The key never leaves your phone's
  secure hardware. Voice notes are kept inside that same database.
- We do not show ads, we do not sell anything, and we do not train any AI on what you
  write. Nightjar has no AI features at all.
- **Nothing leaves your phone at all** — no crash reports, no diagnostics, no analytics.
- **You can speak a dream instead of typing it, and the recording stays on your phone.**
  Nothing in this version turns speech into text, and no recording is ever sent to a
  transcription service.
- Because your dreams are only on your phone, **if you lose the phone, they are gone.**
  Use Export to keep a copy somewhere you choose. The export holds your dream text and
  its details — it does **not** hold your voice recordings, and the file it makes is not
  encrypted.
- To delete everything: **Settings → Data → "Erase everything"**, confirmed by typing
  `IŠTRINTI`. Two settings survive it on purpose — see §7, which names them.

### Trumpai (lietuviškai)

Tavo sapnai lieka telefone — mes jų nematome, nes nėra nei paskyros, nei serverio.
Žurnalas laikomas šifruotoje duomenų bazėje, raktas nepalieka telefono saugios
aparatinės dalies. Balso įrašai saugomi toje pačioje šifruotoje bazėje kaip sapno
tekstas ir ištrinami kartu su sapnu; kol įrašas daromas, garso failas trumpam guli
nešifruotas programėlės privačioje saugykloje, o grojant failas ištrinamas dar prieš
prasidedant garsui ir įrašas skamba iš programėlės atminties. Mikrofono Android paprašo
pirmą kartą paspaudus „įrašyti" — pati programėlė niekada neįrašinėja savavališkai.
Reklamos nėra, duomenų neparduodame, AI funkcijų programėlė neturi. **Iš telefono
neišeina niekas** — nei strigčių ataskaitos, nei diagnostika, nei analitika. **Šioje
versijoje kalba į tekstą neverčiama** — sapną gali pasakyti balsu, ir įrašas lieka
telefone, bet niekas jo netranskribuoja ir jokiai atpažinimo tarnybai nesiunčia. Kadangi
sapnai yra tik telefone, praradus telefoną jie dingsta: naudokis eksportu. Į eksporto
failą įeina sapnų tekstas ir jų detalės, bet **neįeina balso įrašai**, o pats failas
nešifruotas. Viską ištrinti: **Nustatymai → Duomenys → „Ištrinti viską"**, patvirtinant
įrašius `IŠTRINTI`.

---

## 1. Who is responsible for your data

**E-HANDEL OG UTVIKLING BANCEVICIUS**, organisasjonsnummer **930963550**, Herman Grans
vei 57b, 5162 Bergen, Norway, is the data controller for the limited processing described
in this policy. You can reach us about privacy at **tomas.Bance@gmail.com**.

## 2. The short answer: what leaves your phone

Almost nothing.

Nightjar has **no user accounts, no cloud sync, no server of our own, no advertising,
no analytics and no AI features.** We cannot read your dreams. This is not a promise
about how carefully we handle your journal — it is a statement that we never receive it.

Everything below is the detail behind that sentence.

## 3. What stays on your phone

These never leave your device, and we never see them:

- The title and text of every dream you write.
- The date and time of each entry.
- Your tags, emotions, and lucid / nightmare markers.
- Your voice recordings, kept inside that same encrypted database.
- The search index built from your entries.
- Your reminder time, your PIN and your biometric setting.

**How they are protected.** The journal is stored in a SQLite database encrypted with
SQLCipher. The encryption key is generated on your device the first time you open the
app and is kept in the Android Keystore — hardware-backed secure storage. The key is
never transmitted anywhere, and it is not included in any backup. If you turn on the
PIN or biometric lock, the journal will not open without it.

Protection has limits, and we would rather say so than imply otherwise: a device that
is unlocked and in someone else's hands, or a rooted or malware-infected device, is
outside what any app's encryption can defend against.

**Voice recordings.** Nightjar can record a spoken dream and keep it with the entry. A
saved recording is stored in the same encrypted database as the dream text, on your device
only, and is deleted together with the dream.

Android asks for the microphone the first time you press record — not when you install the
app and not when you open it. Nightjar never records unless you press record: there is no
background recording and no automatic recording.

While a recording is being made, the audio file exists unencrypted in the app's private
storage. It is deleted as soon as the recording is saved, and also if the recording fails
or you discard it. If the app is killed while recording, the leftover file is deleted the
next time you open Nightjar.

Playing a recording back works differently, and the difference is worth stating plainly.
The file written for playback is deleted **before** the sound starts, and the recording
plays from the app's own memory instead. So during playback the audio is unencrypted **in
memory** rather than on disk: no other app can reach it through Android's sandbox, it
touches no file, and it is gone when the app closes.

During both of those windows the audio is protected by Android's app sandbox and by your
device's lock screen, not by Nightjar's encryption. On many phones the device storage is
encrypted as well, but Nightjar supports Android 7 and newer and cannot promise that for
every phone it runs on — so we do not.

**About the microphone permission.** The Play listing shows that Nightjar can use the
microphone, and the reason is the recording described above — that is the only thing in
this version that uses it. Nightjar does not transcribe what you say, and no audio is sent
anywhere: see §5.

## 3a. The morning reminder

Nightjar can wake you at a time you choose, so the dream is written down while you still
have it. This is **off until you turn it on**, and Android will ask your permission for
notifications at that moment — not when you first open the app.

The reminder is an ordinary alarm set on your own phone. It does not go through Google's
push service or any server of ours, and nothing about it leaves the device — not the time
you picked, not whether you use it, not whether you wrote anything that morning.

**The reminder never quotes your journal.** Its words are fixed, they are the same for
everybody, and there is no way for a dream — or a count of your dreams, or the date of your
last one — to appear in them. This is deliberate and it is not only about your lock screen:
Android stores the text of a scheduled notification in a plain, unencrypted file, so a
sentence from your journal placed in a reminder would leave the encrypted database and stay
on disk in readable form. So we made it impossible to put one there rather than promising
not to.

The time you choose is stored in the encrypted database with everything else, and erasing
everything cancels the reminder before it deletes anything — you will not be woken by an
app whose contents you have just destroyed.

## 3b. The questions we ask you, once

After you save your first dream, Nightjar asks you a short set of questions. Not before —
you can install the app and write a dream without answering anything, and the questions
appear only once that first dream is saved.

**You may see fewer of them than someone else does, and that is not an accident.** A
question we cannot act on is not asked at all: if your phone has no PIN and no fingerprint
set up, we do not ask about locking the journal. The counter you see ("1 of 2") counts the
questions you will actually be asked, not the questions that exist. In this version of
Nightjar there is no crash reporting at all, so that question is not asked either.

Each one switches on a feature that already exists:

1. **What time should we remind you?** Sets the morning reminder described in §3a.
2. **Do you want to lock your journal?** Turns on the PIN or biometric lock described
   in §3.

**Every one of them can be skipped**, with a plain button and no second asking. Skipping
is a complete answer: nothing is asked again, nothing is held back, and every one of those
settings stays available in Settings afterwards if you change your mind.

**Your answers stay on this phone.** They are stored in the encrypted database alongside
your dreams, or in your phone's own secure storage. None of them is transmitted anywhere,
because there is nowhere for them to go — there is no account and no server. Erasing
everything removes your reminder time along with the journal; §7 says precisely what
happens to the others, because the honest answer is not "all of it".

**What we do not ask.** There is no question about your age, your gender, your health,
your beliefs, your dreams' content, or how you found the app. §10 explains why that is a
commitment rather than an omission.

## 4. What we send: nothing

**This version of Nightjar sends nothing at all** — no crash reports, no diagnostics, no
analytics. Nothing about your use of the app reaches us or anyone else.

There is no third party receiving anything from this app, and there is no service we could
look your data up in, because none of it was ever sent.

If that ever changes, §11 says what we will do before it does.

## 5. Voice notes and speech-to-text

**This version of Nightjar does not turn speech into text.** You write your dream by
typing it. If you would rather speak it, Nightjar records it as a voice note and keeps
the recording — §3 says exactly what happens to it — but nothing converts it to words.

There is no dictation button, and no part of the app asks a speech service — on your
phone or anywhere else — to transcribe anything. Your recordings are never sent to a
transcription service, ours or anyone else's, because none is used at all.

## 6. Backups

Nightjar is excluded from Android's automatic backup, **and from Android's
phone-to-phone transfer**. Your journal is **not** copied to Google Drive and is not
carried to a new phone, which means nobody — not Google and not us — holds a copy of
it. It also means that if you lose or reset your phone, or move to a new one, your
dreams are gone. If that matters to you, use Export and keep the file somewhere you
control.

Two things to know before you rely on that file. It is **not encrypted**, so anyone who
can open it can read your journal — put it somewhere you trust, not in a shared folder.
And it contains your dream text, dates, tags, emotions and markers, but **not your voice
recordings**: those stay in the encrypted database on this phone. An export restored on
a new phone gives you your written journal back, without the audio.

## 7. Deleting your data

There is no account, so there is nothing for us to delete on our side — we hold nothing.
Deletion is entirely in your hands, and it must actually work:

- **One dream:** delete it in the app. It is removed from the journal, from the search
  index, and its voice recording is deleted with it.
- **Everything:** open **Settings → Data → "Erase everything"**, and confirm by typing the
  word `IŠTRINTI`. This destroys the encryption key as well as the data, so nothing left on
  the device can be recovered. It also removes your reminder time and cancels the morning
  alarm itself.
- **One setting deliberately survives it**, and we would rather name it than let you
  discover it: whether your journal is **locked**. If we asked you that question when you
  first opened the app (§3b), your answer to it is the one that stays. It is a single on/off
  switch — it contains nothing you wrote and nothing about you. It stays on purpose: if
  erasing everything also switched your lock off, the erase would silently *unlock* the app
  on a phone you may be erasing precisely because someone else is about to hold it. You can
  change it in Settings at any time.
- **Uninstalling** the app removes its data from the phone.

Because this version sends nothing anywhere (§4), there are no records held by us or by
anyone else for you to ask us to delete.

See also the [Nightjar data-deletion page](data-deletion.html), which restates this
section in Google Play's own format, including the deletion-request address.

## 8. Your rights

If GDPR applies to you, you have the rights of access, rectification, erasure,
restriction, portability and objection.

You can complain about us to the Norwegian Data Protection Authority (**Datatilsynet**,
`datatilsynet.no`), which supervises us because that is where we are established. You can
also complain to the data protection authority of the country you live in — in Lithuania,
the State Data Protection Inspectorate (Valstybinė duomenų apsaugos inspekcija,
`vdai.lrv.lt`). You do not have to contact us first.

In practice, for almost everything, you exercise these rights yourself and instantly:
your journal is on your phone, you can read it, edit it, delete it and export it to JSON
without asking us — the export covers your dream text and its details, but not your voice
recordings (§6). Since this version transmits nothing, there is no copy of anything held by
us for these rights to reach.

## 9. Children

Nightjar is intended for people aged **16 and over**. It is not directed at children, we
do not knowingly collect anything from a child, and there is nothing in the app for a child
to be collected *from* — there is no account, no profile and no server.

## 10. What Nightjar deliberately does not do

- No advertising, no advertising ID, no ad SDK.
- **No push notifications.** The morning reminder is set on your phone; nothing is sent to
  it from outside. Nightjar has no push token and no server that could message you.
- No analytics, no tracking, no behavioural profiling.
- We do not sell or share your data. There is no data to sell.
- We do not use your dreams to train any model, ours or anyone else's.
- There are no AI features in this version. If we ever add one, it will be off by
  default, it will ask before each use, and this policy will be updated before it ships
  — not after.
- We do not require an account, and we do not ask for your name, e-mail or phone number.
- **No transcription in this version.** Nightjar records a voice note when you ask it to
  (§3), and nothing turns it into text. The app never listens on its own: recording starts
  only when you press record, and stops when you stop it. See §5 — and note that the
  transcription half is a statement about *this* release, not a permanent promise: if
  dictation is switched on later, §5 and the Data Safety declaration change together,
  before it ships.
- **We do not ask you about yourself.** Nightjar never asks your age, your gender, your
  health or sleep problems, your religious, political or philosophical beliefs, your sex
  life, your medication or therapy, your use of alcohol or drugs, or anything about other
  people in your life. Not when you install it, not in the questions in §3b, not
  anywhere. Other dream apps ask most of this in their first few minutes; we decided we
  are not entitled to. The only things Nightjar ever asks you are the ones in §3b, and
  each of them switches on a feature you can also reach in Settings.
- **We do not ask you what your dreams are about, either** — no nightmare frequency, no
  dream types, no goals. You write what you want to write, and nothing in the app
  categorises you from it.

## 11. Changes to this policy

If we change what leaves your phone, we will update this policy and the Google Play Data
Safety declaration together, and tell you in the app before the change takes effect.
The date at the top is the version date.
