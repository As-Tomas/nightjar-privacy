# Nightjar — Deleting your data

Version 1.0 · 2026-09-07 · Nightjar for Android (`io.nightjar.app`)

## There is nothing for us to delete, and that is not a dodge

Nightjar has no accounts. You do not sign in, you never give us an e-mail address or a name, and
there is no server of ours anywhere in the app. Your journal is on your phone and nowhere else.

We hold no copy of your dreams, no backup of them, no snapshot, and no record that you use the app
at all. There is no retention period for us to tell you about either: a retention period is how
long we would keep something, and nothing of yours ever reaches us, so nothing is being kept and
nothing is waiting to expire. Deletion is something you do on your phone, it takes effect
immediately, and it does not need our permission or our help.

**If you still want to send us a deletion request, you can** — write to **tomas.Bance@gmail.com**,
which is the deletion-request address for Nightjar. You do not need the app installed to do it and
you will never be sent back to the app to make a request. We will answer, and the answer will
almost certainly be that we hold nothing of yours to delete.

Below is exactly how deletion works on your phone, and exactly what each path removes.

## Deleting one dream

Delete a dream from the journal in the app. This removes:

- the entry itself — its title, text, date, tags, emotions and its lucid / nightmare markers;
- the entry's voice recording, if it has one, and the temporary playback file if one exists;
- the entry's text from the search index, so it can no longer be found by searching.

It is immediate and it cannot be undone.

## Deleting everything

Open **Settings → Data → "Erase everything"**, and confirm by typing the word **IŠTRINTI**. The
button stays disabled until that word is typed — a mistap cannot start it.

The app then, in this order:

1. cancels the morning reminder, so you are not woken by an app whose contents you have just
   destroyed;
2. **destroys the encryption key** held in your phone's Android Keystore;
3. closes the journal database;
4. deletes the database files;
5. deletes the whole temporary-file area — playback copies of voice recordings, anything left by
   speech handling, and any export file the app had prepared.

Step 2 is the one that matters most, and it is why this is deletion rather than tidying up. Your
journal is stored in a database encrypted with SQLCipher, and the key to it lives in your phone's
secure hardware. Once that key is destroyed, anything that might survive on the storage chip after
step 4 is unreadable — by us, by you, and by anyone with the phone in their hands and the tools to
look. There is no second copy of that key anywhere; it was never transmitted and it was never
included in any backup.

If the app is closed or the phone dies partway through, the erase resumes and finishes the next
time you open Nightjar, and it tells you it did so.

**One setting deliberately survives**, and we would rather name it here than let you find out:
**whether your journal is locked** with a PIN or fingerprint. It is a single on/off switch — it
holds nothing you wrote and nothing about you. It stays on purpose, because an erase that silently
switched your lock off would unlock the app on a phone you may be erasing precisely because someone
else is about to hold it. You can change it in Settings at any time.

This is a real deletion, not a deactivation and not a freeze. There is no account to freeze, no
"disabled" state to come back from, and no waiting period.

## What deletion cannot reach

**Files you exported and shared yourself.** If you used Export and sent the file to Drive, Gmail,
a chat, or your own storage, that copy is yours and it is where you put it. Deleting in the app
does not reach it, and neither can we — we never saw it. Delete it wherever you sent it. The export
file is not encrypted, so it is worth doing.

Everything else is covered. There is no cloud copy: Nightjar is excluded from Android's automatic
backup and from Android's phone-to-phone transfer, so your journal is never copied to Google Drive
and never carried to a new phone. There is no AI service holding anything, because the app has no
AI features and sends nothing to any AI provider. There are no crash reports, diagnostics or
analytics to purge, because this version sends none.

## Uninstalling

Uninstalling Nightjar removes its data from the phone. If you want to be certain the encryption key
is destroyed first, use "Erase everything" before you uninstall.

## Contact

E-HANDEL OG UTVIKLING BANCEVICIUS, organisasjonsnummer 930963550, Herman Grans vei 57b, 5162
Bergen, Norway, is the data controller for Nightjar. Privacy and **deletion requests**:
tomas.Bance@gmail.com.

You can ask us anything at that address, including asking us to delete anything you believe we hold
— but for your journal you do not need to, and waiting for a reply would only delay something you
can do yourself in under a minute.

See also the [Nightjar Privacy Policy](https://as-tomas.github.io/nightjar-privacy/), in particular
§7 "Deleting your data".

---

# Nightjar — kaip ištrinti savo duomenis

Versija 1.0 · 2026-09-07 · Nightjar, Android (`io.nightjar.app`)

## Mums nėra ko trinti, ir tai ne išsisukinėjimas

Nightjar neturi paskyrų. Neprisijungi, nenurodai nei el. pašto, nei vardo, ir programėlėje nėra
jokio mūsų serverio. Tavo žurnalas yra telefone ir daugiau niekur.

Mes neturime nei tavo sapnų kopijos, nei atsarginės kopijos, nei jokio įrašo, kad apskritai
naudojiesi programėle. Nėra ir saugojimo termino, kurį galėtume nurodyti: saugojimo terminas — tai
kiek laiko ką nors laikytume, o pas mus tavo duomenys niekada nepatenka, tad niekas nėra laikoma ir
niekas nelaukia, kol pasibaigs terminas. Trynimas vyksta tavo telefone, įsigalioja iškart, ir jam
nereikia nei mūsų leidimo, nei pagalbos.

**Jei vis dėlto nori atsiųsti prašymą ištrinti duomenis — gali.** Rašyk **tomas.Bance@gmail.com**;
tai Nightjar duomenų trynimo prašymų adresas. Programėlės tam turėti nereikia, ir niekada nebūsi
nusiųstas atgal į programėlę, kad pateiktum prašymą. Atsakysime — ir atsakymas beveik neabejotinai
bus toks, kad jokių tavo duomenų neturime.

Žemiau — tiksliai kaip trynimas veikia telefone ir ką kiekvienas kelias pašalina.

## Vieno sapno trynimas

Ištrink sapną žurnale. Bus pašalinta:

- pats įrašas — pavadinimas, tekstas, data, žymos, emocijos, sąmoningo sapno ir košmaro žymekliai;
- to sapno balso įrašas, jei jis yra, ir laikinas grojimo failas, jei toks buvo;
- to sapno tekstas iš paieškos rodyklės, tad paieška jo daugiau neras.

Veiksmas įsigalioja iškart ir yra negrįžtamas.

## Viską ištrinti

Atidaryk **Nustatymai → Duomenys → „Ištrinti viską"** ir patvirtink įrašydamas žodį **IŠTRINTI**.
Kol žodis neįrašytas, mygtukas neaktyvus — netyčia paspausti neįmanoma.

Tada programėlė šia tvarka:

1. atšaukia rytinį priminimą, kad tavęs nežadintų programėlė, kurios turinį ką tik sunaikinai;
2. **sunaikina šifravimo raktą**, saugomą telefono Android Keystore;
3. uždaro žurnalo duomenų bazę;
4. ištrina duomenų bazės failus;
5. ištrina visą laikinų failų sritį — grojimui iššifruotas balso įrašų kopijas, tai, ką paliko
   kalbos apdorojimas, ir eksporto failą, jei toks buvo paruoštas.

Svarbiausias yra antras žingsnis, ir būtent dėl jo tai yra trynimas, o ne tvarkymasis. Žurnalas
laikomas SQLCipher šifruota duomenų baze, o raktas į ją guli telefono saugioje aparatinėje dalyje.
Sunaikinus raktą, kas nors ir liktų atminties luste po ketvirto žingsnio, yra neperskaitoma — nei
mums, nei tau, nei tam, kas laikytų telefoną rankose ir mokėtų ieškoti. Antros to rakto kopijos
niekur nėra: jis niekada nebuvo perduotas ir niekada nepateko į jokią atsarginę kopiją.

Jei programėlė užsidarytų ar telefonas išsijungtų vidury trynimo, jis bus tęsiamas ir užbaigtas kitą
kartą atidarius Nightjar — ir programėlė apie tai pasakys.

**Vienas nustatymas sąmoningai išlieka**, ir mes verčiau jį įvardysime, nei leisime aptikti: ar
žurnalas užrakintas PIN kodu arba pirštu. Tai vienas įjungimo/išjungimo jungiklis — jame nėra nieko,
ką rašei, ir nieko apie tave. Jis lieka tyčia: trynimas, kuris tyliai išjungtų užraktą, atrakintų
programėlę telefone, kurį galbūt kaip tik dėl to ir trini, kad jis tuoj atsidurs svetimose rankose.
Nustatymuose gali jį pakeisti bet kada.

Tai tikras ištrynimas, o ne deaktyvavimas ir ne užšaldymas. Nėra paskyros, kurią būtų galima
užšaldyti, nėra „išjungtos" būsenos, į kurią būtų galima grįžti, ir nėra jokio laukimo laikotarpio.

## Ko trynimas nepasiekia

**Failų, kuriuos pats eksportavai ir išsiuntei.** Jei pasinaudojai eksportu ir nusiuntei failą į
Drive, Gmail, pokalbį ar savo saugyklą — ta kopija yra tavo ir yra ten, kur ją padėjai. Trynimas
programėlėje jos nepasiekia, ir mes irgi ne — mes jos niekada nematėme. Ištrink ją ten, kur
nusiuntei. Eksporto failas nešifruotas, tad verta tai padaryti.

Visa kita padengta. Debesyje kopijos nėra: Nightjar išbraukta iš Android automatinių atsarginių
kopijų ir iš perkėlimo į naują telefoną, tad žurnalas niekada nepatenka nei į Google Drive, nei į
naują telefoną. Nėra AI tarnybos, kuri ką nors laikytų — programėlė neturi AI funkcijų ir nieko
jokiam AI tiekėjui nesiunčia. Nėra ir strigčių ataskaitų, diagnostikos ar analitikos, kurią reikėtų
šalinti: ši versija jų nesiunčia.

## Pašalinus programėlę

Pašalinus Nightjar, jos duomenys iš telefono dingsta. Jei nori būti tikras, kad pirma sunaikintas
šifravimo raktas, prieš šalindamas pasinaudok „Ištrinti viską".

## Kontaktai

Nightjar duomenų valdytojas — E-HANDEL OG UTVIKLING BANCEVICIUS, organisasjonsnummer 930963550,
Herman Grans vei 57b, 5162 Bergen, Norvegija. Privatumo klausimais ir **prašymams ištrinti
duomenis**: tomas.Bance@gmail.com.

Tuo adresu gali klausti bet ko, taip pat ir paprašyti ištrinti tai, ką, tavo manymu, turime — bet
dėl savo žurnalo tau to daryti nereikia, o laukimas atsakymo tik uždelstų tai, ką pats padarysi per
nepilną minutę.

Taip pat žr. [Nightjar privatumo politiką](https://as-tomas.github.io/nightjar-privacy/), ypač §7
„Deleting your data".
