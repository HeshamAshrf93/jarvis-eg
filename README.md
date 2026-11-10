# jarvis-eg

A voice assistant that understands Egyptian Arabic commands and controls a 3D scene: "كبّر المجسم"، "لف لليمين"، "فكّ الموتور".

> Status: early development.

## Planned features

- [ ] Speech-to-text for Egyptian Arabic (pluggable providers)
- [ ] An LLM turns the spoken command into a structured action (rotate, zoom, explode, load model, reset)
- [ ] Clear list of allowed actions, validated in code, so the assistant can't do anything outside it
- [ ] Spoken replies in Egyptian Arabic (text-to-speech)
- [ ] Wake word ("يا جارفس")
- [ ] Works together with gesture control (e.g. stark-hands) through a shared events API
- [ ] Mixed Arabic/English commands ("zoom in شوية")
- [ ] Automated tests with text commands written for this project

## Planned usage

```bash
pip install -r requirements.txt
cp .env.example .env   # add your own API keys, never commit them
python -m jarvis_eg
```

## Roadmap

1. Project setup: packaging, tests, CI
2. Text command to action (LLM + validation)
3. Speech-to-text
4. Text-to-speech replies
5. Wake word
6. Events API for 3D scene control
7. Mixed language commands
8. Docs and demo

## Privacy

Voice recordings are not stored. Test data is text written for this project.

## License

MIT, see [LICENSE](LICENSE).

---
Built by [Hesham Ashraf](https://www.linkedin.com/in/hesham-ashrf)
