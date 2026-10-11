# Participant Recruitment Website

Static participant recruitment page for the multilingual speech-emotion study.

## Languages

- English: `/?lang=en`
- Japanese: `/?lang=ja`
- Indonesian: `/?lang=id`

## Preview locally

From this folder:

```bash
python3 -m http.server 8080
```

Then open:

- http://localhost:8080/?lang=en
- http://localhost:8080/?lang=ja
- http://localhost:8080/?lang=id

## Before publishing

Open `app.js` and edit:

```js
const CONFIG = {
  researcherName: "[Researcher name]",
  researcherEmail: "[Research email]"
};
```

Do not add compensation, room numbers, recruitment deadlines, or other study details unless they are included in the approved study documents.

## Structure

- `index.html` — page structure
- `styles.css` — academic/Kyutech-inspired styling
- `app.js` — EN/JA/ID translations and contact configuration

This recruitment page is intentionally separate from the experiment application.
It does not expose M1/M2/M3, model probabilities, researcher-only controls, or participant data.


## Registration form

The site uses the Google Form URL configured in `app.js`:

```js
registrationFormUrl: "https://forms.gle/ZDJ3mPbwzC1neqTZ8"
```

The registration form is separate from formal informed consent.
