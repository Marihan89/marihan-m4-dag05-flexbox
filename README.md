# Dag 5 · Flexbox

*Modul 4, UI/UX & Frontendutveckling, Lexicon IT-Proffs*

## Vad du ska göra idag

Du lägger ut menyn, sidhuvudet och sidfoten med Flexbox, och lär dig skillnaden mellan huvudaxel och korsaxel.

## Bakgrund

Flexbox ordnar element i **en dimension**: en rad eller en kolumn. Du sätter `display: flex` på **parent**, och children ordnar sig. Det är samma tänk som Auto layout i Figma, och du har redan gjort det i modul 3.

## Så arbetar du (samma som alltid)

1. **Forka** dagens repo på GitHub (*Fork → Create fork*).
2. **Klona din fork:** *Code → HTTPS → kopiera adressen*. I terminalen (Ctrl+ö i VS Code): `git clone <adressen>`. Öppna den nya mappen i VS Code och starta *Live Server*.
3. **Gör uppgiften.** Spara och kontrollera i webbläsaren efter varje steg. Gör en commit efter varje avslutat steg: `git add .` och `git commit -m "Beskriv vad du gjorde"`.
4. **Skicka upp** när du är klar: `git push`.
5. **Lämna in i Microsoft Forms.**

Fastnar du: skriv ner exakt var och vad du försökt, och ta det först i nästa handledda pass.

## Uppgiften steg för steg

### Steg 1. Menyn på rad

`nav ul` ska visa länkarna på en rad med `display: flex` och `gap: 20px`. Testa sedan `flex-direction: column` och byt tillbaka.

### Steg 2. Sidhuvudet med justering

Gör `header` till en flexbehållare. Rubriken ska ligga till vänster och menyn till höger (`justify-content: space-between`), vertikalt centrerade (`align-items: center`). Lägg till `flex-wrap: wrap` så att det bryter snyggt när det är trångt.

### Steg 3. Sidfoten

Samma teknik: copyrightraden till vänster, adressen till höger, med `gap` för luft.

### Steg 4. Kort med jämn höjd

Gör `article` till en flexbehållare i kolumn (`flex-direction: column`). Ge `.pris` `margin-top: auto` så att priset alltid hamnar längst ned i kortet, oavsett textlängd.

### Steg 5. Experimentera

I DevTools: ändra `justify-content` till `center`, `flex-end`, `space-around`. Ändra `align-items`. Skriv i en kommentar vad varje värde gör, med egna ord.

### Steg 6. Rita axlarna

Rita på papper en flexrad och en flexkolumn och märk ut *huvudaxel* och *korsaxel*. Skriv vilken egenskap som styr var och en.

## Kontrollista: så vet du att du är klar

- [ ] Menyn, sidhuvudet och sidfoten är byggda med Flexbox.
- [ ] Du har använt `gap` istället för marginaler mellan flex items.
- [ ] Priset ligger längst ned i varje kort.
- [ ] `flex-wrap: wrap` finns där det behövs, och sidan går inte sönder på smal skärm.
- [ ] Du kan förklara huvudaxel och korsaxel.
- [ ] Du har pushat till din fork och skickat in länken.

## Tips om du fastnar

- Inget händer? `display: flex` ska på PARENT, inte på children.
- `justify-content` och `align-items` byter roller när du ändrar `flex-direction`. Det är normalt.
- Använd DevTools: klicka på `flex`-ikonen bredvid elementet, så ritas axlarna ut.

## Inlämning

**Deadline: imorgon klockan 09.00.** Allt lämnas in i Microsoft Forms. Du behöver inte redovisa något muntligt.

I formuläret fyller du i:

1. Länk till din fork av det här repot.
2. Reflektion: Vilken Flexbox-egenskap var mest förvirrande, och hur skulle du förklara den för en kollega?

## Vill du mer? (frivilligt)

- Gör menyn till en hamburgarmeny-liknande layout för smal skärm med enbart CSS.
- Använd `flex-grow` för att låta ett fält i formuläret fylla resten av raden.

_______________________________________________________________________________________________
# Day 5 · Flexbox

*Module 4, UI/UX & Frontend Development, Lexicon IT-Proffs*

## What to do today

You will lay out the menu, header and footer with Flexbox, and learn the difference between the main axis and the cross axis.

## Background

Flexbox arranges elements in **one dimension**: a row or a column. You set `display: flex` on **parent**, and children arrange themselves. It is the same idea as Auto layout in Figma, and you have already done it in module 3.

## How to work (same as always)

1. **Fork** today's repo on GitHub (*Fork → Create fork*).
2. **Clone your fork:** *Code → HTTPS → copy the address*. In the terminal (Ctrl+ö in VS Code): `git clone <address>`. Open the new folder in VS Code and start *Live Server*.
3. **Do the task.** Save and check in the browser after each step. Make a commit after each completed step: `git add .` and `git commit -m "Describe what you did"`.
4. **Submit** when you are finished: `git push`.
5. **Submit in Microsoft Forms.**

If you get stuck: write down exactly where and what you tried, and take it first in the next supervised session.

## The task step by step

### Step 1. The menu on a line

`nav ul` should display the links on a line with `display: flex` and `gap: 20px`. Then test `flex-direction: column` and change back.

### Step 2. The header with alignment

Make `header` a flex container. The title should be on the left and the menu on the right (`justify-content: space-between`), vertically centered (`align-items: center`). Add `flex-wrap: wrap` so it wraps nicely when it's crowded.

### Step 3. Footer

Same technique: copyright line on the left, address on the right, with `gap` for air.

### Step 4. Cards with even height

Make `article` a flex container in column (`flex-direction: column`). Give `.price` `margin-top: auto` so that the price always ends up at the bottom of the card, regardless of text length.

### Step 5. Experiment

In DevTools: change `justify-content` to `center`, `flex-end`, `space-around`. Change `align-items`. Write in a comment what each value does, in your own words.

### Step 6. Draw the axes

Draw a flex row and a flex column on paper and label them *main axis* and *cross axis*. Write which property controls each.

## Checklist: how to know you're done

- [ ] The menu, header and footer are built with Flexbox.
- [ ] You've used `gap` instead of margins between flex items.
- [ ] The price is at the bottom of each card.
- [ ] `flex-wrap: wrap` is where it's needed, and the page doesn't break on narrow screens.
- [ ] You can explain the main axis and cross axis.
- [ ] You've pushed to your fork and submitted the link.

## Tips if you get stuck

- Nothing happens? `display: flex` should be on PARENT, not on children.
- `justify-content` and `align-items` switch roles when you change `flex-direction`. This is normal.
- Use DevTools: click on the `flex` icon next to the element, and the axes will be drawn.

## Submission

**Deadline: tomorrow at 09:00.** Everything is submitted in Microsoft Forms. You do not need to present anything verbally.

In the form, fill in:

1. Link to your fork of this repo.

2. Reflection: Which Flexbox feature was the most confusing, and how would you explain it to a colleague?

## Want more? (optional)

- Make the menu a hamburger-like layout for narrow screens using only CSS.

- Use `flex-grow` to let a field in the form fill the rest of the row.
