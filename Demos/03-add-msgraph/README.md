# <a name="how-to-run-the-completed-project"></a><span data-ttu-id="6026a-101">Exécution du projet terminé</span><span class="sxs-lookup"><span data-stu-id="6026a-101">How to run the completed project</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6026a-102">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="6026a-102">Prerequisites</span></span>

<span data-ttu-id="6026a-103">Pour exécuter le projet terminé dans ce dossier, vous avez besoin des éléments suivants:</span><span class="sxs-lookup"><span data-stu-id="6026a-103">To run the completed project in this folder, you need the following:</span></span>

- <span data-ttu-id="6026a-104">[Python](https://www.python.org/) (avec [PIP](https://pypi.org/project/pip/)) installé sur votre ordinateur de développement.</span><span class="sxs-lookup"><span data-stu-id="6026a-104">[Python](https://www.python.org/) (with [pip](https://pypi.org/project/pip/)) installed on your development machine.</span></span> <span data-ttu-id="6026a-105">Si vous n'avez pas python, visitez le lien précédent pour obtenir les options de téléchargement.</span><span class="sxs-lookup"><span data-stu-id="6026a-105">If you do not have Python, visit the previous link for download options.</span></span> <span data-ttu-id="6026a-106">(**Remarque:** ce didacticiel a été écrit avec Python version 3.7.0 et Django version 2,1.</span><span class="sxs-lookup"><span data-stu-id="6026a-106">(**Note:** This tutorial was written with Python version 3.7.0 and Django version 2.1.</span></span> <span data-ttu-id="6026a-107">Les étapes de ce guide peuvent fonctionner avec d'autres versions, mais cela n'a pas été testé.)</span><span class="sxs-lookup"><span data-stu-id="6026a-107">The steps in this guide may work with other versions, but that has not been tested.)</span></span>
- <span data-ttu-id="6026a-108">Soit un compte Microsoft personnel avec une boîte aux lettres sur Outlook.com, soit un compte professionnel ou scolaire Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6026a-108">Either a personal Microsoft account with a mailbox on Outlook.com, or a Microsoft work or school account.</span></span>

<span data-ttu-id="6026a-109">Si vous n'avez pas de compte Microsoft, vous disposez de deux options pour obtenir un compte gratuit:</span><span class="sxs-lookup"><span data-stu-id="6026a-109">If you don't have a Microsoft account, there are a couple of options to get a free account:</span></span>

- <span data-ttu-id="6026a-110">Vous pouvez vous [inscrire pour obtenir un nouveau compte Microsoft personnel](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span><span class="sxs-lookup"><span data-stu-id="6026a-110">You can [sign up for a new personal Microsoft account](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span></span>
- <span data-ttu-id="6026a-111">Vous pouvez vous [inscrire au programme pour les développeurs office 365](https://developer.microsoft.com/office/dev-program) pour obtenir un abonnement gratuit à Office 365.</span><span class="sxs-lookup"><span data-stu-id="6026a-111">You can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

## <a name="register-a-web-application-with-the-azure-active-directory-admin-center"></a><span data-ttu-id="6026a-112">Enregistrer une application Web avec le centre d'administration Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6026a-112">Register a web application with the Azure Active Directory admin center</span></span>

1. <span data-ttu-id="6026a-113">Ouvrez un navigateur et accédez au [Centre d'administration Azure Active Directory](https://aad.portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="6026a-113">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="6026a-114">Connectez-vous à l'aide d'un compte **personnel** (alias Microsoft) ou **compte professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="6026a-114">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="6026a-115">Sélectionnez **Azure Active Directory** dans le volet de navigation de gauche, puis sélectionnez **inscriptions des applications (aperçu)** sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="6026a-115">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations (Preview)** under **Manage**.</span></span>

    ![<span data-ttu-id="6026a-116">Capture d'écran des inscriptions d'application</span><span class="sxs-lookup"><span data-stu-id="6026a-116">A screenshot of the App registrations</span></span> ](/tutorial/images/aad-portal-app-registrations.png)

1. <span data-ttu-id="6026a-117">Sélectionnez **nouvelle inscription**.</span><span class="sxs-lookup"><span data-stu-id="6026a-117">Select **New registration**.</span></span> <span data-ttu-id="6026a-118">Sur la page **inscrire une application** , définissez les valeurs comme suit.</span><span class="sxs-lookup"><span data-stu-id="6026a-118">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="6026a-119">Définissez **nom** sur `Python Graph Tutorial`.</span><span class="sxs-lookup"><span data-stu-id="6026a-119">Set **Name** to `Python Graph Tutorial`.</span></span>
    - <span data-ttu-id="6026a-120">Définissez les types de comptes **pris en charge** sur **les comptes de tous les comptes d'annuaire et de Microsoft personnels**.</span><span class="sxs-lookup"><span data-stu-id="6026a-120">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="6026a-121">Sous **URI**de redirection, définissez la première liste déroulante sur `Web` et définissez la `http://localhost:8000/tutorial/callback`valeur sur.</span><span class="sxs-lookup"><span data-stu-id="6026a-121">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:8000/tutorial/callback`.</span></span>

    ![Capture d'écran de la page inscrire une application](/tutorial/images/aad-register-an-app.png)

1. <span data-ttu-id="6026a-123">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="6026a-123">Choose **Register**.</span></span> <span data-ttu-id="6026a-124">Sur la page **didacticiel Graph de Python** , copiez la valeur de l' **ID d'application (client)** et enregistrez-la, vous en aurez besoin à l'étape suivante.</span><span class="sxs-lookup"><span data-stu-id="6026a-124">On the **Python Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Capture d'écran de l'ID d'application de la nouvelle inscription de l'application](/tutorial/images/aad-application-id.png)

1. <span data-ttu-id="6026a-126">Sélectionnez **certificats & secrets** sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="6026a-126">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="6026a-127">Sélectionnez le bouton **nouveau client secrète** .</span><span class="sxs-lookup"><span data-stu-id="6026a-127">Select the **New client secret** button.</span></span> <span data-ttu-id="6026a-128">Entrez une valeur dans **Description** , puis sélectionnez l'une des options \*\*\*\* pour expirer, puis choisissez **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="6026a-128">Enter a value in **Description** and select one of the options for **Expires** and choose **Add**.</span></span>

    ![Capture d'écran de la boîte de dialogue Ajouter une clé secrète client](/tutorial/images/aad-new-client-secret.png)

1. <span data-ttu-id="6026a-130">Copiez la valeur de la clé secrète client avant de quitter cette page.</span><span class="sxs-lookup"><span data-stu-id="6026a-130">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="6026a-131">Vous en aurez besoin à l'étape suivante.</span><span class="sxs-lookup"><span data-stu-id="6026a-131">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="6026a-132">Cette clé secrète client ne s'affiche plus, vérifiez que vous la copiez maintenant.</span><span class="sxs-lookup"><span data-stu-id="6026a-132">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![Capture d'écran de la clé secrète client récemment ajoutée](/tutorial/images/aad-copy-client-secret.png)

## <a name="configure-the-sample"></a><span data-ttu-id="6026a-134">Configurer l'exemple</span><span class="sxs-lookup"><span data-stu-id="6026a-134">Configure the sample</span></span>

1. <span data-ttu-id="6026a-135">Renommez `oauth_settings.yml.example` le fichier `oauth_settings.yml`.</span><span class="sxs-lookup"><span data-stu-id="6026a-135">Rename the `oauth_settings.yml.example` file to `oauth_settings.yml`.</span></span>
1. <span data-ttu-id="6026a-136">Modifiez le `oauth_settings.yml` fichier et effectuez les modifications suivantes.</span><span class="sxs-lookup"><span data-stu-id="6026a-136">Edit the `oauth_settings.yml` file and make the following changes.</span></span>
    1. <span data-ttu-id="6026a-137">Remplacez `YOUR_APP_ID_HERE` par l' **ID d'application** que vous avez obtenu à partir du portail d'inscription des applications.</span><span class="sxs-lookup"><span data-stu-id="6026a-137">Replace `YOUR_APP_ID_HERE` with the **Application Id** you got from the App Registration Portal.</span></span>
    1. <span data-ttu-id="6026a-138">Remplacez `YOUR_APP_PASSWORD_HERE` par le mot de passe que vous avez obtenu à partir du portail d'inscription des applications.</span><span class="sxs-lookup"><span data-stu-id="6026a-138">Replace `YOUR_APP_PASSWORD_HERE` with the password you got from the App Registration Portal.</span></span>
1. <span data-ttu-id="6026a-139">Dans votre interface de ligne de commande (CLI), accédez à ce répertoire et exécutez la commande suivante pour installer les conditions requises.</span><span class="sxs-lookup"><span data-stu-id="6026a-139">In your command-line interface (CLI), navigate to this directory and run the following command to install requirements.</span></span>

    ```Shell
    pip install -r requirements.txt
    ```

1. <span data-ttu-id="6026a-140">Dans votre interface CLI, exécutez la commande suivante pour initialiser la base de données de l'application.</span><span class="sxs-lookup"><span data-stu-id="6026a-140">In your CLI, run the following command to initialize the app's database.</span></span>

    ```Shell
    python manage.py migrate
    ```

## <a name="run-the-sample"></a><span data-ttu-id="6026a-141">Exécution de l’exemple</span><span class="sxs-lookup"><span data-stu-id="6026a-141">Run the sample</span></span>

1. <span data-ttu-id="6026a-142">Exécutez la commande suivante dans votre interface CLI pour démarrer l'application.</span><span class="sxs-lookup"><span data-stu-id="6026a-142">Run the following command in your CLI to start the application.</span></span>

    ```Shell
    python manage.py runserver
    ```

1. <span data-ttu-id="6026a-143">Ouvrez un navigateur et accédez à `http://localhost:8000/tutorial`.</span><span class="sxs-lookup"><span data-stu-id="6026a-143">Open a browser and browse to `http://localhost:8000/tutorial`.</span></span>