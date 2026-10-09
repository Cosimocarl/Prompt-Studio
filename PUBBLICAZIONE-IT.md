# Pubblicare Prompt Studio su GitHub

## 1. Crea una nuova repository

Apri https://github.com/new e scegli:

- Nome: `prompt-studio` (puoi sceglierne un altro: cambierà l’URL).
- Visibilità: **Public**.
- Non aggiungere README, licenza o .gitignore in questa schermata: il pacchetto contiene già il README.

Premi **Create repository**.

## 2. Carica i file

Estrai `Prompt-Studio-GitHub.zip`. Apri la cartella `prompt-studio` e carica **il suo contenuto**, non la cartella contenitore e non il file ZIP.

Nella nuova repository usa **uploading an existing file**, oppure **Add file → Upload files**. Trascina `index.html`, `README.md`, `PUBBLICAZIONE-IT.md` e le cartelle `assets` e `docs`. Conferma con **Commit changes**.

Nella pagina principale della repository devi vedere direttamente `index.html`. Se è dentro `prompt-studio/index.html`, hai caricato un livello di cartella in più: sposta i file alla radice prima di proseguire.

## 3. Attiva il sito

Vai in **Settings → Pages**. In **Build and deployment**:

1. **Source:** `Deploy from a branch`.
2. **Branch:** `main` (o il nome effettivo del ramo dove hai caricato i file).
3. **Folder:** `/ (root)`.
4. Premi **Save**.

Aspetta che la pubblicazione termini. Controlla **Actions** se compare un errore. In **Settings → Pages** apparirà il link del sito e il pulsante **Visit site**.

L’indirizzo sarà `https://TUO-USERNAME.github.io/prompt-studio/`; sostituisci `TUO-USERNAME` con il tuo nome GitHub. Se hai scelto un altro nome per la repository, sostituisci anche `prompt-studio`.

## 4. Rendi il sito facile da trovare

Nella pagina principale della repository, vicino a **About**, premi l’ingranaggio e incolla il link reale nel campo **Website**.

Puoi anche modificare il README aggiungendo, con il tuo URL reale:

```markdown
[Apri Prompt Studio](https://TUO-USERNAME.github.io/prompt-studio/)
```

GitHub mostra il README e il codice. Il prodotto interattivo si usa sul link GitHub Pages. I visitatori del sito non hanno bisogno di un account GitHub.

## 5. Chi può modificare cosa

Non invitare altri utenti come collaboratori con permessi di scrittura se vuoi mantenere il controllo della versione pubblicata. I visitatori possono usare l’app e salvare prompt nel proprio browser senza cambiare il sito condiviso.

La repository pubblica espone il codice, che può essere scaricato o copiato. Non è possibile impedirne tecnicamente la modifica in una copia privata. Il proprietario può sempre aggiornare la repository e i relativi permessi: questo pacchetto non introduce un blocco irreversibile per te.

## Verifica dopo la pubblicazione

- Apri il link Pages e controlla che compaia l’app, non il README.
- Cambia lingua, scegli un’attività e carica un esempio.
- Compila il brief, copia il prompt e prova l’esportazione.
- Salva un prompt e ricarica la pagina: deve essere nella raccolta di quel browser.
- Apri il sito in una finestra privata: non deve mostrare la raccolta della sessione normale.

Per trasferire i salvataggi dal vecchio HTML locale al sito, esporta il backup JSON dal vecchio file e importalo nel sito.

## Documentazione ufficiale

- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/repository-access-and-collaboration/permission-levels-for-a-personal-account-repository
