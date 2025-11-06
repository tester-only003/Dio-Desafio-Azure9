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
   <img width="436" height="286" alt="Modify-effect1" src="https://github.com/user-attachments/assets/b5c235d2-6c35-495a-a437-6504ad59a51e" />
   </div>

<br>

  > A policy tem algumas condições ou estados, por exemplo, você pode criar uma policy, deixar ela pronta como se estivesse desativada (foi criada mas não está ativa).
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











