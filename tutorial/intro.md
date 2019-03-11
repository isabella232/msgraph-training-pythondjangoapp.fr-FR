<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="8882a-101">Ce didacticiel vous apprend à créer une application Web python django qui utilise l'API Microsoft Graph pour récupérer des informations de calendrier pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8882a-101">This tutorial teaches you how to build a Python Django web app that uses the Microsoft Graph API to retrieve calendar information for a user.</span></span>

> [!TIP]
> <span data-ttu-id="8882a-102">Si vous préférez télécharger simplement le didacticiel terminé, vous pouvez le télécharger de deux manières.</span><span class="sxs-lookup"><span data-stu-id="8882a-102">If you prefer to just download the completed tutorial, you can download it in two ways.</span></span>
>
> - <span data-ttu-id="8882a-103">Téléchargez le [démarrage rapide de Python](https://developer.microsoft.com/graph/quick-start?platform=option-Python) pour obtenir du code de travail en quelques minutes.</span><span class="sxs-lookup"><span data-stu-id="8882a-103">Download the [Python quick start](https://developer.microsoft.com/graph/quick-start?platform=option-Python) to get working code in minutes.</span></span>
> - <span data-ttu-id="8882a-104">Téléchargez ou clonez le [référentiel GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp).</span><span class="sxs-lookup"><span data-stu-id="8882a-104">Download or clone the [GitHub repository](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8882a-105">Conditions requises</span><span class="sxs-lookup"><span data-stu-id="8882a-105">Prerequisites</span></span>

<span data-ttu-id="8882a-106">Avant de commencer ce didacticiel, [python](https://www.python.org/) (avec [PIP](https://pypi.org/project/pip/)) doit être installé sur votre ordinateur de développement.</span><span class="sxs-lookup"><span data-stu-id="8882a-106">Before you start this tutorial, you should have [Python](https://www.python.org/) (with [pip](https://pypi.org/project/pip/)) installed on your development machine.</span></span> <span data-ttu-id="8882a-107">Si vous n'avez pas python, visitez le lien précédent pour obtenir les options de téléchargement.</span><span class="sxs-lookup"><span data-stu-id="8882a-107">If you do not have Python, visit the previous link for download options.</span></span>

> [!NOTE]
> <span data-ttu-id="8882a-108">Ce didacticiel a été écrit avec Python version 3.7.0 et Django version 2,1.</span><span class="sxs-lookup"><span data-stu-id="8882a-108">This tutorial was written with Python version 3.7.0 and Django version 2.1.</span></span> <span data-ttu-id="8882a-109">Les étapes de ce guide peuvent fonctionner avec d'autres versions, mais cela n'a pas été testé.</span><span class="sxs-lookup"><span data-stu-id="8882a-109">The steps in this guide may work with other versions, but that has not been tested.</span></span>

## <a name="feedback"></a><span data-ttu-id="8882a-110">Commentaires</span><span class="sxs-lookup"><span data-stu-id="8882a-110">Feedback</span></span>

<span data-ttu-id="8882a-111">Veuillez fournir des commentaires sur ce didacticiel dans le [référentiel GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp).</span><span class="sxs-lookup"><span data-stu-id="8882a-111">Please provide any feedback on this tutorial in the [GitHub repository](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp).</span></span>