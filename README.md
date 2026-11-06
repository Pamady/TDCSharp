# Boutique Diayma
Boutique Diayma : TD .NET (Visual Studio, débogage)

Papa Amady Diallo - M2 - GLSI - ESP
Lien github : https://github.com/Pamady/TDCSharp
Lien drvie de l'executable : https://drive.google.com/file/d/1yW5b5nWjtj5hTQ4OFfvyezhZ293TgJHW/view?usp=sharing


1. Récupération et exécution du code
Dépôt cloné dans Visual Studio, solution Diayma.sln ouverte.
Fenêtre d'avertissement NuGet fermée. Elle signale des packages vulnérables.
Problème rencontré au premier lancement : erreur 0x80008096, car le runtime .NET Core 2.1 n'était pas insallé.

Application lancée avec succès.


2. Projets de la solution
La solution Diayma.sln contient un seul projet : Diayma (fichier P2FixAnAppDotNetCode/Diayma.csproj)

3. Version du SDK .NET utilisée
Le projet ne fixe pas de version de SDK (pas de global.json). Il cible le framework .NET Core 2.0 (netcoreapp2.0).

4. Installation du SDK / runtime
Déjà installé.

5. Dépôt GitHub personnel
Dépôt créé : https://github.com/Pamady/TDCSharp

6. Bugs trouvés
Bug 1 : le total du panier ignore les quantités
Bug 2 : le stock ne diminue pas après une commande

7. Points d'arrêt posés

8. Parcours du code avant l'affichage des produits
	1.
		Namespace : P2FixAnAppDotNetCode
		Classe : Startup
		Méthode : le constructeur Startup(IConfiguration configuration)
		F10 (Pas à pas principal) : exécute la ligne 20 et passe à la ligne 21
	2.
		Namespace : P2FixAnAppDotNetCode.Controllers
		Classe : ProductController
		Méthodes : ProductContrller, productService
		F11 (Pas à pas dtaillé)

	3.
		Namespace : P2FixAnAppDotNetCode.Components
		Classe : CartSummaryViewComponent
		Méthode : Invoke
		F10 (Pas à pas principal)


9 et 10. Lien drive de l'executable
https://drive.google.com/file/d/1yW5b5nWjtj5hTQ4OFfvyezhZ293TgJHW/view?usp=sharing