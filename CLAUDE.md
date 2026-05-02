# StrategyThrust Dashboard

GitHub Pages uzerinde static outreach dashboard. Outreach pipeline'dan gelen email verilerini gosterir, onay/red mekanizmasi sunar.

## Structure

```
strategythrust-dashboard/
  index.html              - Tek sayfa dashboard (HTML/CSS/JS)
  strategythrust_logo.png - Logo
  data/
    emails.json           - Pipeline'dan gelen email verileri
```

## How It Works

- GitHub Pages'te host ediliyor (sertacgul/strategythrust-dashboard)
- data/emails.json, outreach pipeline'in sync_to_github.py scripti ile push ediliyor
- Onay/red kararlari GitHub Gist'teki approvals.json uzerinden yurutuluyor
- Data cekme: GitHub blob API ile (cache bypass, size limit yok)

## Related Project

- **Outreach Pipeline**: C:\Users\serta\strategythrust-outreach
  - Email uretimi, firma analizi, gonderim islemleri orada yapiliyor
  - Bu dashboard sadece gosterim ve onay katmani

## Rules

- Em-dash ve en-dash kullanma, sadece kisa hyphen (-)
- ActLedger projesiyle karistirma, tamamen ayri proje
