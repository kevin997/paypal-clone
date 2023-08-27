Il s'agit d'un projet [Next.js](https://nextjs.org/) démarré avec [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

La commande suivante a été utilisée pour créer ce projet

```bash
npx create-next-app@latest paypal-clone--typescript --tailwind --eslint

```

# Clonage et Branching

Assurez-vous d'avoir téléchargé [Git](https://git-scm.com/) sur votre machine.

Pour ceux qui ont Linux, faites une recherche sur Google pour savoir comment installer Git sur votre distribution Linux.

la branche par défaut est `main`. vous ne devez jamais envoyer vos modifications à cette branche.

Lorsque vous clonez ce dépôt avec la commande : `git clone https://github.com/kevin997/paypal-clone.git`,

Allez dans le projet clone avec : `cd paypal-clone`, puis lister les branches locales avec : `git branch`. Cette commande vous donnera une liste des branches sur votre PC.

Pour commencer à travailler sur une nouvelle branche, entrez ce qui suit dans le terminal : `git checkout -b Le nom de votre branche`.

### Veuillez noter : ☝🏽 le nom de votre branche doit être le nom de la (des) fonction(s) sur laquelle (lesquelles) vous voulez travailler, par exemple `authentication`, `send-money`, `add-money-to-wallet`.

Une fois que vous avez terminé de travailler sur une fonctionnalité, vous devez la télécharger dans le référentiel en ligne afin que votre tuteur puisse corriger votre code et faire des suggestions. Voici comment procéder :

``git add .``` 👈🏽 ceci ajoutera toutes vos modifications au système de contrôle de version (VCS)


``git commit -m "votre message"`` 👈🏽 ceci créera une instance historique de votre code source. le message peut être une courte description de ce que vous avez modifié. Notez que le "" doit être présent


git push -u Votre nom de branche 👈🏽 ceci créera votre branche sur le dépôt en ligne

si cette commande ne fonctionne pas, utilisez :

git push -u --set-upstream-to=votre nom de branche votre nom de branche

ou simplement ``git push`` 👈🏽 git vous donnera une erreur mais avec une suggestion de ce qu'il faut faire.



### Sur le dépôt en ligne, créez une Pull Request (PR) pour intégrer les changements de votre branche à la branche `main`. Je viendrai l'approuver.



### Démarrage

Après avoir créé une nouvelle branche locale, allez à la racine de votre projet et créez un fichier d'environnement

```bash
sous Windows : copier .env.example .env

sur linux ou max : cp .env.example .env
```

Initialisez ces variables avec les vôtres, puis exécutez la commande ci-dessous pour installer les dépendances nécessaires à ce projet :

```bash
npm install

#ou
yarn install

#ou

pnpm install
```

Après l'installation, assurez-vous d'avoir un dossier prisma et un fichier schema.prisma, car il s'agit d'un [ORM](https://fr.wikipedia.org/wiki/Mapping_objet-relationnel) 👈🏽 cliquez ici pour la définition

C'est avec ce fichier schema.prisma que vous allez créer et gérer vos tables.


Pour avoir une idée de ce à quoi ressemble votre application web NextJs, exécutez les commandes ci-dessous :

Tout d'abord, lancez le serveur de développement :

```bash
npm run dev
# ou
yarn dev
# ou
pnpm dev
```

Ouvrez [http://localhost:3000](http://localhost:3000) avec votre navigateur pour voir le résultat.

Vous pouvez commencer à éditer la page en modifiant `app/page.tsx`. La page se met à jour automatiquement au fur et à mesure que vous modifiez le fichier.

Ce projet utilise [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) pour optimiser et charger automatiquement Inter, une police Google personnalisée.

# En savoir plus

Pour en savoir plus sur Next.js, consultez les ressources suivantes :

- [Next.js Documentation](https://nextjs.org/docs) - pour en savoir plus sur les fonctionnalités et l'API de Next.js.
- Learn Next.js](https://nextjs.org/learn) - un tutoriel interactif sur Next.js.

Vous pouvez consulter [le dépôt Next.js GitHub](https://github.com/vercel/next.js/) - vos commentaires et contributions sont les bienvenus !

# Déployer sur Vercel

La façon la plus simple de déployer votre application Next.js est d'utiliser la [Plate-forme Vercel](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) des créateurs de Next.js.

Consultez notre [documentation sur le déploiement de Next.js](https://nextjs.org/docs/deployment) pour plus de détails.