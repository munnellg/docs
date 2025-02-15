---
title: Tornar um aplicativo do GitHub público ou privado
intro: '{% data reusables.shortdesc.making-a-github-app-public-or-private %}'
redirect_from:
  - /apps/building-integrations/setting-up-and-registering-github-apps/about-installation-options-for-github-apps/
  - /apps/building-github-apps/installation-options-for-github-apps/
  - /apps/building-integrations/managing-github-apps/changing-a-github-app-s-installation-option/
  - /apps/managing-github-apps/changing-a-github-app-s-installation-option/
  - /apps/managing-github-apps/making-a-github-app-public-or-private
versions:
  free-pro-team: '*'
  enterprise-server: '*'
  github-ae: '*'
topics:
  - GitHub Apps
---

Para obter informações de autenticação, consulte "[Efetuando autenticação com aplicativos GitHub](/apps/building-github-apps/authenticating-with-github-apps/#authenticating-as-an-installation)".

### Fluxo público de instalação

Os fluxos de instalação pública têm uma página inicial para permitir que outras pessoas, além do proprietário do aplicativo, instalem o aplicativo nos seus repositórios. Este link é fornecido no campo "Link público" ao configurar seu aplicativo GitHub. Para obter mais informações, consulte "[Instalando aplicativos GitHub](/apps/installing-github-apps/)".

### Fluxo privado de instalação

Os fluxos privados de instalação permitem que somente o proprietário de um aplicativo GitHub a instale. Informações limitadas sobre o GitHub App continuarão a existir em uma página pública, mas o botão **Instalar** só estará disponível para administradores da organização ou para a conta de usuário se o aplicativo GitHub for propriedade de uma conta individual. Private{% if currentVersion ver_lt "enterprise-server@3.2" or currentVersion == "github-ae@latest" %}, or internal,{% endif %} GitHub Apps can only be installed on the user or organization account of the owner.

### Alterar quem pode instalar seu aplicativo GitHub

Para alterar quem pode instalar o aplicativo GitHub:

{% data reusables.user-settings.access_settings %}
{% data reusables.user-settings.developer_settings %}
{% data reusables.user-settings.github_apps %}
3. Selecione o aplicativo GitHub cuja opção de instalação você deseja alterar. ![Seleção de aplicativo](/assets/images/github-apps/github_apps_select-app.png)
{% data reusables.user-settings.github_apps_advanced %}
5. Depending on the installation option of your GitHub App, click either **Make public** or **Make {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@3.1" %}private{% else %}internal{% endif %}**. ![Botão para alterar a opção de instalação do seu aplicativo GitHub](/assets/images/github-apps/github_apps_make_public.png)
6. Depending on the installation option of your GitHub App, click either **Yes, make this GitHub App public** or **Yes, make this GitHub App {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@3.1" %}private{% else %}internal{% endif %}**. ![Botão para confirmar a mudança de sua opção de instalação](/assets/images/github-apps/github_apps_confirm_installation_option.png)
