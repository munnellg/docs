---
title: Enterprise アカウントについて
intro: '{% data variables.product.prodname_ghe_cloud %} では Enterprise アカウントを作り、Organization 間のコラボレーションを可能にしながら、管理者は一カ所で可視性と管理を扱えるようにできます。'
product: '{% data reusables.gated-features.enterprise-accounts %}'
redirect_from:
  - /articles/about-github-business-accounts/
  - /articles/about-enterprise-accounts
  - /github/setting-up-and-managing-your-enterprise-account/about-enterprise-accounts
versions:
  free-pro-team: '*'
  enterprise-server: '*'
topics:
  - Enterprise
---

### Enterprise アカウントについて

Enterprise アカウントでは、複数の {% data variables.product.prodname_dotcom %} Organization と {% data variables.product.prodname_ghe_server %} インスタンスを管理できます。 Enterprise アカウントは、{% data variables.product.prodname_dotcom %} 上の Organization や個人アカウントのようにハンドルを持たなければなりません。 Enterprise 管理者は、以下のような設定やプリファレンスを管理できます:

- メンバーのアクセスと管理 (Organization のメンバー、外部コラボレーター)
- 支払いと使用状況（{% data variables.product.prodname_ghe_server %} インスタンス、ユーザライセンス、{% data variables.large_files.product_name_short %} パック{% if currentVersion == "free-pro-team@latest" or ver_gt "enterprise-server@3.0" %}、{% data variables.product.prodname_GH_advanced_security %} の使用状況{% endif %}）
- セキュリティ (シングルサインオン、2 要素認証)
- {% data variables.contact.enterprise_support %} とのリクエストおよび Support Bundle の共有

{% data reusables.enterprise-accounts.enterprise-accounts-billing %}{% data variables.product.prodname_ghe_cloud %} サブスクリプションの管理に関する詳しい情報については、「[Enterprise アカウントのサブスクリプションと利用状況の表示](/articles/viewing-the-subscription-and-usage-for-your-enterprise-account)」を参照してください。 {% data variables.product.prodname_ghe_server %} の支払い設定の管理に関する詳しい情報については、「[Enterprise の支払いの管理](/admin/overview/managing-billing-for-your-enterprise)」を参照してください。

{% data variables.product.prodname_ghe_cloud %} と {% data variables.product.prodname_ghe_server %} の違いについては、「[{% data variables.product.prodname_dotcom %} の製品](/articles/githubs-products)」を参照してください。 {% data variables.product.prodname_enterprise %} にアップグレードする、または Enterprise アカウントを使い始める場合は、{% data variables.contact.contact_enterprise_sales %} にお問い合わせください。

メンバーのアクセスと管理の詳細については、「{% if currentVersion == "free-pro-team@latest" %}[Enterprise 内のユーザを管理する](/github/setting-up-and-managing-your-enterprise/managing-users-in-your-enterprise){% elsif currentVersion == "enterprise-ae@latest" or enterpriseServerVersions contains currentVersion %}[ユーザ、Organization、リポジトリを管理する](/admin/user-management)」を参照してください{% endif %}。

GraphQL APIを利用したEnterpriseアカウントの管理に関する詳しい情報については、「[Enterprise アカウント](/graphql/guides/managing-enterprise-accounts)」を参照してください。

{% if currentVersion == "free-pro-team@latest" %}

### Enterprise アカウントにリンクされた Organization を管理する

Organization は、多くの人がいくつものプロジェクトにわたって同時にコラボレーションできる共有アカウントです。 オーナーは、Organization のデータとプロジェクトへのメンバーのアクセスを、洗練されたセキュリティおよび管理機能で管理できます。 詳細は「[Organization について](/articles/about-organizations)」を参照してください。

Enterprise のオーナーは、Organization を作成して Enterprise にリンクできます。 Organization を Enterprise アカウントに追加した後は、Organization のポリシーを管理して強制できます。 特定の強制の選択肢は、設定によって異なります。概して、Enterprise アカウント内のすべての Organization に単一のポリシーを強制するか、Organization レベルでオーナーがポリシーを設定することを許可するかを選択できます。

詳細は「[Enterprise アカウントで Organization を管理する](/articles/managing-organizations-in-your-enterprise-account)」および「[Enterprise アカウント内の Organization に対するポリシーを設定する](/articles/setting-policies-for-organizations-in-your-enterprise-account)」を参照してください。

{% endif %}

### Enterprise アカウントにリンクされている {% data variables.product.prodname_ghe_server %} ライセンスの管理

{% data reusables.enterprise-accounts.admin-managing-licenses %}
