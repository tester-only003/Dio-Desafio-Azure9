# Primeiros Passos com Governança e Conformidade na Azure

## Blueprints, Políticas e Bloqueio de Recursos

### Governança e Conformidade
- Blueprints, políticas e bloqueios de recursos
- Portal de Confiança do Serviço

**OBJETIVOS:**
- Descrever a finalidade do Azure Policy.
- Descrever a finalidade dos bloqueios de recurso.
- Descrever a finalidade do Portal de Confiança do Serviço.
- Descrever a finalidade do Microsoft Purview.

<br>

### Azure Policy
O <ins> Azure Policy ajuda a impor padrões organizacionais</ins> e a avaliar a conformidade em escala.
  - Ele fornece governança e consistência de recursos com conformidade regulatória, segurança, custo e gerenciamento.

- *A policy não determina por pessoa (usuário), determina por organização. Impõe padrões seja a quem for (independente do nível de usuário).*
<br>

- Avalia e identifica os recursos do Azure que não atendem às suas políticas.
- Fornece definições de políticas e iniciativas integradas, em categorias como armazenamento, rede, computação, central de segurança e monitoramento.
<br>

   <div align="center">
   <img width="336" height="286" alt="Modify-effect1" src="https://github.com/user-attachments/assets/b5c235d2-6c35-495a-a437-6504ad59a51e" />
   </div>

<br>

> [!NOTE] 
> A policy tem algumas condições ou estados, por exemplo, você pode criar uma policy, deixar ela pronta como se estivesse desativada (foi criada mas não está ativa).
 [!NOTE]
<br>

#### *Non-compliant: 
   Não está atendendo ao requisito. <br>
   *A policy não afeta recursos existentes. Por mais que ela esteja ativada, todos os outros recursos criados estão dentro de um padrão, ela não muda o efeito daquilo que já existe.*

#### *Remediation: 
  Tudo o que existe eu quero que seja validado e o que não está no conforme eu quero que seja ajustado. <br>
  *Será feito uma alteração de estado daquilo (o recurso) que já existe. <br>
  Necessário ter atenção caso for alterar o que já está ativo, para não trazer um cenário de indisponibilidade.*
<br>

#### Compliant: 
Todos os itens que respondem para determinada policy, seguem os padrões esperados. <br>

A policy tanto avalia como determina se o recurso que está sendo criado, ou que já foi, segue ou não aquilo que a policy determina.
<br>
<br>

> [!NOTE] 
> Lembrando: quando falamos de policy, não falamos de usuários, estamos nos referindo ao gerenciamento de recursos (padronização dos recursos). [!NOTE]
<br>


### Gerenciando Bloqueio de Recursos


#### Bloqueio de Recursos
- Proteja os recursos do Azure de exclusão ou modificação acidental.
- Gerenciar bloqueios da assinatura, grupo de recursos ou níveis de recursos individuais dentro do Portal do Azure.
<br>

> [!NOTE] 
> *Bloqueio de Recursos servem quando precisamos manter o estado ou garantir a não exclusão de um recurso que esteja (por exemplo) em uma assinatura ou em um Resource Group.*  [!NOTE]

<br>

> [!IMPORTANT] 
> Se eu colocar um bloqueio à nível de Resource Group, tudo o que estiver dentro deste resource group herdará este bloqueio. <br>
Bloqueio são herdáveis ao contrário das Tags. <br>
**Bloqueio sempre cai na prova do AZ900.**
[!IMPORTANT]

<br>

   <div align="center">
   <img width="709" height="155" alt="Tipo-bloqueio1" src="https://github.com/user-attachments/assets/594c44da-a984-442c-aded-e4f181b24f53" />

   </div>
<br>

O tipo de bloqueio que infere menor ação será sempre o de excluir, porque eu consigo ler e consigo atualizar.
<br>
<br>

> [!WARNING] 
> *Se um recurso recebe um bloqueio por estar em um Resource Group, quando ele é movido para outro Resource Group ele não leva esse bloqueio com ele. [!WARNING]
<br>

#### Portal de Confiança do Serviço
Um link aberto ao público onde são disponibilizadas as informações de conformidade e segurança (útil, por exemplo, para auditorias).
<br>
<br>

#### Microsoft Purview
O Microsoft Purview é uma família de soluções de <ins> **governança, risco e conformidade de dados** </ins> que ajuda você a obter uma única exibição unificada em seus dados. O Microsoft Purview reúne insights sobre seus dados locais, multinuvem e de software como serviço.
<br>
  - Avalia estratégias de compliance.
    - Informa quem pode ter acesso e alterar as informações, por exemplo.
<br>
- Descoberta de dados automatizada. <br>
- Classificação de dados confidenciais. <br>
- Linhagem de dados de ponta a ponta. <br>

<br>

#### Portal de Confiança - Certificações, regulamentos e padrões
https://servicetrust.microsoft.com/

<br>

#### Revisão Governança e Conformidade

[https://learn.microsoft.com/en-us/purview/purview](https://learn.microsoft.com/en-us/purview/purview)

[https://learn.microsoft.com/training/modules/describe-cost-management-azure/1-introduction](https://learn.microsoft.com/training/modules/describe-cost-management-azure/1-introduction)

[https://learn.microsoft.com/training/modules/describe-features-tools-azure-for-governance-compliance/3-describe-purpose-of-azure-policy](https://learn.microsoft.com/training/modules/describe-features-tools-azure-for-governance-compliance/3-describe-purpose-of-azure-policy)

[https://learn.microsoft.com/training/modules/describe-features-tools-azure-for-governance-compliance/4-describe-purpose-of-resource-locks](https://learn.microsoft.com/training/modules/describe-features-tools-azure-for-governance-compliance/4-describe-purpose-of-resource-locks)















