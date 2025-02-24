# Moveto Studio - Solutions IA Sectorielles

## 🎯 Vision et Stratégie

Moveto est un studio de solutions IA sectorielles qui combine expertise technique et connaissance métier pour créer des plateformes intelligentes spécialisées. Notre approche unique permet de déployer rapidement des solutions verticales complètes pour différents secteurs d'activité.

### Vision Technologique
```mermaid
graph TB
    subgraph "Expertise Technique"
        RAG[RAG/LLM Avancé]
        ARCH[Architecture Scalable]
        INFRA[Infrastructure Cloud]
    end

    subgraph "Produits"
        CHAT[Agents Conversationnels]
        GEN[Générateurs de Contenu]
        INFO[Systèmes d'Information]
    end

    subgraph "Services"
        AGENT[Création d'Agents IA]
        SRC[Intégration Sources]
        PERSO[Personnalisation]
    end

    subgraph "Verticaux"
        SANTE[Formation Santé]
        TECH[Formation Tech]
        FIN[Formation Finance]
        FUTUR[Autres Secteurs...]
    end

    RAG --> CHAT
    RAG --> GEN
    ARCH --> INFO
    INFRA --> PERSO
    
    CHAT --> SANTE
    GEN --> TECH
    INFO --> FIN
    PERSO --> FUTUR
```

### 🔄 Écosystème Moveto : Passerelle.cc & Flowz.cc

L'écosystème Moveto s'articule autour de deux plateformes complémentaires qui forment un cycle complet d'intelligence et d'action :

```mermaid
graph LR
    subgraph "Passerelle.cc"
        RAG[RAG Dual]
        AGENTS[Agents Spécialisés]
        ANALYSE[Analyse Sectorielle]
        INSIGHTS[Insights Personnalisés]
    end
    
    subgraph "Flowz.cc"
        SCRAPING[Scraping Intelligent]
        WORKFLOW[Workflow Automatisé]
        CRM[CRM Intelligent]
        ACTION[Automatisation Actions]
    end
    
    %% Flux d'intégration
    RAG --> INSIGHTS
    INSIGHTS --> ACTION
    ACTION --> SCRAPING
    SCRAPING --> RAG
    AGENTS --> WORKFLOW
    WORKFLOW --> AGENTS
    ANALYSE --> CRM
    CRM --> ANALYSE
    
    %% Styles
    classDef passerelle fill:#9370DB,stroke:#9370DB,color:#fff
    classDef flowz fill:#FF7E67,stroke:#FF7E67,color:#fff
    
    class RAG,AGENTS,ANALYSE,INSIGHTS passerelle
    class SCRAPING,WORKFLOW,CRM,ACTION flowz
```

#### Passerelle.cc : La Plateforme d'Analyse
- **Compréhension contextuelle** des données sectorielles
- **Analyse personnalisée** des documents utilisateurs
- **Insights intelligents** via RAG dual
- **Agents spécialisés** par domaine d'expertise

#### Flowz.cc : La Plateforme d'Action
- **Scraping Intelligent** : Collecte automatisée de données avec IA
- **Workflow Intelligent** : Automatisation des processus métier
- **CRM Intelligent** : Gestion et qualification des leads B2B
- **Mise en action** des insights générés par Passerelle.cc

#### Synergie et Intégration
Cette approche intégrée permet de créer un cycle vertueux où :
1. **Passerelle.cc analyse** les données sectorielles et documents utilisateurs
2. **Flowz.cc collecte** de nouvelles données pertinentes
3. **Passerelle.cc génère** des insights actionnables
4. **Flowz.cc automatise** les actions basées sur ces insights

### 🚀 Vision Future : Agents IA Verticaux

Selon une [étude de Y Combinator](https://www.ycombinator.com/library/Lt-vertical-ai-agents-could-be-10x-bigger-than-saas), les agents IA verticaux pourraient représenter un marché 10 fois plus important que le SaaS traditionnel. Moveto s'inscrit pleinement dans cette vision avec une feuille de route ambitieuse :

#### 1. Transformation en Système Multi-Agents Autonome
- Agents spécialisés par tâche et secteur
- Orchestration automatique des workflows
- Réduction drastique de l'intervention humaine
- Prise de décision autonome basée sur les données

#### 2. Infrastructure B2A (Business-to-Agent)
- API publique pour l'intégration avec d'autres systèmes
- Système de plugins extensible
- Outils de monitoring et scaling des agents
- Marketplace d'agents spécialisés

#### 3. Automatisation Complète des Processus Métier
- Création automatique des dossiers de certification
- Mise à jour automatique des référentiels
- Validation automatique de la conformité
- Génération de rapports et analyses prédictives

#### 4. Expansion Verticale Multi-Sectorielle
Après le secteur de la formation professionnelle, Moveto prévoit d'étendre son approche à d'autres verticaux :
- Santé et bien-être
- Finance et assurance
- Immobilier
- Ressources humaines
- Éducation supérieure

Cette vision s'appuie sur notre architecture modulaire et notre expertise en RAG, permettant une adaptation rapide à de nouveaux secteurs tout en maintenant une base technologique commune.

### Solutions
1. **Licence Secteur**
   - Solution complète par vertical
   - Personnalisation possible
   - Support dédié
   - Déploiement cloud ou on-premise

2. **Services Pro**
   - Création d'agents personnalisés
   - Intégration de sources spécifiques
   - Formation et accompagnement
   - Conseil en stratégie IA

3. **API/SaaS**
   - IndexManager as a Service
   - Agent Factory API
   - Data Pipeline API
   - Analytics et monitoring

### Innovation ![Innovation](https://img.shields.io/badge/-Innovation-blue)
- Framework RAG++ propriétaire
- IndexManager avec support vectoriel natif
- Architecture multi-agents spécialisée
- Génération de contenu contextuelle
- Infrastructure cloud optimisée
- Système de cache intelligent

### Extensibilité 

Le système est conçu pour être facilement étendu à de nouveaux secteurs :

```python
# Exemple d'extension à un nouveau secteur
class SectorConfig:
    def __init__(self, name: str, sources: List[Source], agents: List[Agent]):
        self.name = name
        self.sources = sources  # Sources de données spécifiques au secteur
        self.agents = agents    # Agents spécialisés
        self.indexes = []       # Index Meilisearch dédiés

    async def initialize(self):
        # Configuration automatique des index
        for source in self.sources:
            index_config = await IndexManager.create_index_config(source)
            self.indexes.append(index_config)
        
        # Déploiement des agents
        for agent in self.agents:
            await agent.deploy()

# Utilisation
tech_sector = SectorConfig(
    name="Formation Tech",
    sources=[
        GitHubTrendsSource(),
        StackOverflowSource(),
        TechCertificationsSource()
    ],
    agents=[
        TechCareerAgent(),
        SkillsAnalysisAgent(),
        LearningPathAgent()
    ]
)
```

Cette architecture permet de :
- Ajouter de nouvelles sources de données
- Créer des agents spécialisés
- Configurer des index dédiés
- Personnaliser les workflows
- Adapter les modèles LLM

## 📊 Plateforme Passerelle.cc

Passerelle.cc est notre première implémentation verticale, spécialisée dans le secteur de la formation professionnelle.

### Architecture

```mermaid
graph TB
    %% Frontend & Infrastructure
    Frontend[Frontend SaaS]
    Coolify[Coolify Deploy]
    CloudflareTunnel[Cloudflare Tunnel]
    CloudflareWorker[Cloudflare Worker]
    Supabase[(Supabase<br/>Users DB)]
    Stripe[Stripe<br/>Payments]
    
    %% Backend Core
    API[API Gateway]
    Redis[(Redis Cache)]
    Meilisearch[(Meilisearch)]
    
    %% Specialized Agents Layer
    BlogGeneratorAgent[Blog Generator<br/>Agent]
    AssistantAgent[Assistant Agent]
    DocumentProcessor[Document<br/>Processor Agent]
    AgentSantePublic[Agent Santé<br/>Public]
    PDFAgent[PDF Agent]
    ChatbotCreator[Chatbot<br/>Creator]
    
    %% Search Orchestrator & Agents
    SearchOrchestrator{Search<br/>Orchestrator}
    SearchAgent[Search Agent]
    RelevanceAgent[Relevance Agent]
    RefinementAgent[Refinement Agent]
    LiveSearchAgent[Live Search Agent]
    CPFLiveSearchAgent[CPF Live<br/>Search Agent]
    
    %% Indexation Agents
    RetourEmploiAgent[RetourEmploi<br/>Agent]
    CPFAgent[CPF Agent]
    DataImportAgent[Data Import<br/>Agent]
    
    %% External APIs
    CPF[CPF API]
    FranceTravail[France Travail API]
    
    %% User Document Vault
    UserDocumentVault[(User Document<br/>Vault)]
    DocumentChunks[(Document<br/>Chunks)]
    
    %% Token Buckets
    RedisTokenBucket[Redis Token<br/>Bucket]
    MeiliTokenBucket[Meilisearch<br/>Token Bucket]
    
    %% Infrastructure Connections
    Frontend --> Coolify
    Coolify --> CloudflareTunnel
    CloudflareTunnel --> API
    Frontend --> CloudflareWorker
    CloudflareWorker --> API
    
    %% Frontend Connections
    Frontend --> Supabase
    Frontend --> Stripe
    
    %% Backend Flow - CORRECTED
    API --> BlogGeneratorAgent
    API --> AssistantAgent
    API --> DocumentProcessor
    API --> AgentSantePublic
    API --> PDFAgent
    API --> ChatbotCreator
    API --> RetourEmploiAgent
    API --> CPFAgent
    API --> DataImportAgent
    
    %% Agent Orchestration
    BlogGeneratorAgent --> SearchOrchestrator
    AssistantAgent --> SearchOrchestrator
    DocumentProcessor --> SearchOrchestrator
    AgentSantePublic --> SearchOrchestrator
    PDFAgent --> SearchOrchestrator
    
    %% Search Orchestrator Flow
    SearchOrchestrator --> |Coordinates| SearchAgent
    SearchOrchestrator --> |Coordinates| RelevanceAgent
    SearchOrchestrator --> |Coordinates| RefinementAgent
    SearchOrchestrator --> |Coordinates| LiveSearchAgent
    SearchOrchestrator --> |Coordinates| CPFLiveSearchAgent
    
    %% Data Sources
    SearchAgent --> Meilisearch
    LiveSearchAgent --> FranceTravail
    CPFLiveSearchAgent --> CPF
    RetourEmploiAgent --> FranceTravail
    CPFAgent --> CPF
    
    %% Cache
    SearchAgent --> Redis
    LiveSearchAgent --> Redis
    CPFLiveSearchAgent --> Redis
    
    %% User Document RAG Flow
    Supabase --> UserDocumentVault
    DocumentProcessor --> UserDocumentVault
    UserDocumentVault --> DocumentChunks
    DocumentChunks --> AssistantAgent
    AssistantAgent --> |User-specific RAG| UserDocumentVault
    
    %% Token Bucket Flow
    RedisTokenBucket <--> MeiliTokenBucket
    DocumentProcessor --> RedisTokenBucket
    SearchAgent --> MeiliTokenBucket
    RetourEmploiAgent --> RedisTokenBucket
    CPFAgent --> RedisTokenBucket
    DataImportAgent --> RedisTokenBucket
    
    %% Styling
    classDef userRag fill:#9370DB,stroke:#9370DB,color:#fff
    classDef bucket fill:#4B0082,stroke:#4B0082,color:#fff
    classDef indexAgent fill:#FF7E67,stroke:#FF7E67,color:#fff
    
    class UserDocumentVault,DocumentChunks userRag
    class RedisTokenBucket,MeiliTokenBucket bucket
    class RetourEmploiAgent,CPFAgent,DataImportAgent indexAgent
```

### Composants Principaux

#### Frontend
- **Supabase** : Gestion des utilisateurs et authentification
- **Stripe** : Gestion des paiements et abonnements

#### Backend Core
- **API Gateway** : Point d'entrée unique pour les requêtes
- **Redis** : Cache pour les résultats de recherche
- **Meilisearch** : Moteur de recherche vectorielle
- **User Document Vault** : Stockage sécurisé des documents utilisateurs
- **Document Chunks** : Fragments de documents vectorisés pour le RAG utilisateur

#### Agents

##### Agents Publics (Interface Utilisateur)
- **AssistantAgent** : Agent principal d'interaction avec l'utilisateur, intègre le RAG dual
- **AgentSantePublic** : Spécialisé dans le domaine de la santé publique
- **PDFAgent** : Traitement et analyse des documents PDF
- **BlogGeneratorAgent** : Génération de contenu pour les blogs

##### Agents d'Orchestration
- **SearchOrchestrator** : Coordonne les différents agents de recherche
- **ChatbotCreator** : Création et configuration de nouveaux agents conversationnels

##### Agents de Recherche et Analyse
- **SearchAgent** : Recherche dans les index Meilisearch
- **RelevanceAgent** : Évalue la pertinence des résultats via RAG
- **RefinementAgent** : Affine les recherches pour améliorer la précision
- **LiveSearchAgent** : Enrichit les résultats via l'API France Travail
- **CPFLiveSearchAgent** : Enrichit les résultats via l'API CPF

##### Agents de Traitement de Documents
- **DocumentProcessor** : Traite et indexe les documents utilisateurs pour le RAG personnalisé
- **DocumentProcessorService** : Service de traitement asynchrone des documents

##### Agents d'Indexation
- **RetourEmploiAgent** : Indexation des données de retour à l'emploi
- **CPFAgent** : Indexation des formations CPF
- **DataImportAgent** : Importation et indexation des données sectorielles

### 🔄 Système RAG Dual

Le système Passerelle.cc intègre une architecture RAG (Retrieval Augmented Generation) à deux niveaux :

#### 1. RAG Global (Sectoriel)
- Basé sur les données sectorielles indexées dans Meilisearch
- Alimenté par les agents d'import (Data Import, Actualités, RetourEmploi, CPF)
- Fournit une base de connaissances commune à tous les utilisateurs
- Optimisé pour les requêtes générales sur le secteur de la formation

#### 2. RAG Utilisateur (Personnalisé)
- Basé sur les documents personnels stockés dans le Vault utilisateur
- Géré par le Document Processor Agent
- Stockage sécurisé dans Supabase avec isolation par utilisateur
- Permet des réponses contextualisées aux données spécifiques de l'utilisateur

#### Fonctionnement
1. Les documents utilisateurs sont téléchargés via le frontend et stockés dans Supabase
2. Le Document Processor Agent traite ces documents :
   - Extraction du texte
   - Chunking (découpage en fragments)
   - Vectorisation
   - Stockage des chunks dans la table document_chunks
3. Lors d'une requête utilisateur, l'Assistant Agent :
   - Interroge le RAG global pour les connaissances sectorielles
   - Interroge simultanément le RAG utilisateur pour les informations personnalisées
   - Fusionne les résultats pour une réponse complète et contextualisée

Cette architecture permet une personnalisation poussée tout en maintenant une base de connaissances commune, offrant ainsi le meilleur des deux mondes aux utilisateurs.

### 🔒 Système de Double Bucket pour les Embeddings

Une innovation majeure de Passerelle.cc est son système de double bucket pour la gestion des embeddings, qui assure une utilisation optimale des ressources et une protection contre les limitations d'API.

```mermaid
graph TB
    subgraph "Système de Double Bucket"
        subgraph "BaseAgent Bucket"
            RB[RedisTokenBucket]
            RF[Redis Flow Control]
            RP[Rate Protection]
        end
        
        subgraph "IndexManager Bucket"
            TB[TokenBucket]
            EB[Embeddings Batch]
            RL[Rate Limiting]
        end
        
        RB <--> TB
        RF --> EB
        RP --> RL
    end
    
    subgraph "Utilisations"
        ME[(Meilisearch<br/>Embeddings)]
        SUP[(Supabase<br/>Document Chunks)]
        DPA[Document<br/>Processor]
        IM[Index<br/>Manager]
    end
    
    TB --> ME
    RB --> SUP
    DPA --> RB
    IM --> TB
    
    %% Styles
    classDef bucket fill:#4B0082,stroke:#4B0082,color:#fff
    classDef component fill:#9370DB,stroke:#9370DB,color:#fff
    
    class RB,TB bucket
    class RF,RP,EB,RL component
```

#### Caractéristiques du Système

1. **Double Couche de Protection**
   - `RedisTokenBucket` dans `agent_base.py` : Gère le flux Redis et la synchronisation avec Meilisearch
   - `TokenBucket` dans `index_manager.py` : Contrôle les appels d'API pour les embeddings

2. **Synchronisation Intelligente**
   - Les deux buckets communiquent pour coordonner les limites de débit
   - Adaptation dynamique aux contraintes des deux systèmes
   - Prévention des erreurs de rate limiting

3. **Optimisation des Ressources**
   - Calcul intelligent du nombre de tokens nécessaires
   - Regroupement des requêtes en lots optimaux
   - Attente adaptative basée sur la disponibilité des tokens

4. **Métriques et Monitoring**
   - Suivi en temps réel de l'utilisation des tokens
   - Statistiques détaillées sur les temps d'attente
   - Alertes en cas d'approche des limites

#### Avantages

- **Fiabilité** : Prévention des erreurs de rate limiting des API externes
- **Performance** : Utilisation optimale des ressources disponibles
- **Économie** : Réduction des coûts liés aux API d'embeddings
- **Scalabilité** : Adaptation automatique aux volumes de données
- **Résilience** : Gestion gracieuse des pics de charge

Ce système est utilisé à la fois pour les embeddings dans Meilisearch (RAG global) et pour les embeddings des documents utilisateurs dans Supabase (RAG utilisateur), garantissant une cohérence et une efficacité optimales dans toute l'architecture.

## 🚀 Architecture Technique Détaillée

```mermaid
graph TB
    subgraph "Infrastructure"
        CFT[Cloudflare Tunnel]
        CFW[Cloudflare Worker]
        COOL[Coolify Deploy]
    end

    subgraph "Frontend"
        UI[UI/UX Layer]
        FRONT[Frontend SaaS]
    end

    subgraph Sources
        API[APIs Externes]
        FC[France Compétences XML]
        FT[France Travail API]
        CPF[CPF API]
    end

    subgraph "Data Pipeline"
        AA[Actualités Agent]
        DA[Data Import Agent]
        REA[RetourEmploi Agent]
        CPFA[CPF Agent]
    end

    subgraph "Search Engine"
        INDM[Index Manager]
        ME[(Meilisearch)]
        subgraph "Indexes"
            RNCP[Fiches RNCP Core]
            TRENDS[Trends]
            REMP[Retour Emploi]
            CPFI[CPF Index]
        end
    end

    subgraph "User Document System"
        SUP[(Supabase DB)]
        DPA[Document Processor Agent]
        subgraph "User Vault"
            UD[User Documents]
            DC[Document Chunks]
            DPS[Document Processing Status]
        end
    end

    subgraph "Cache Layer"
        RE[(Redis)]
        CM[Cache Manager]
    end

    subgraph "Agents Publics"
        subgraph "Agent Components"
            SF[Search & Filters]
            CA[Context Analysis]
            RG[Response Generator]
            SO[Search Orchestrator]
            SA[Search Agent]
            RA[Relevance Agent]
            RF[Refinement Agent]
            LSA[Live Search Agent]
            PDF[PDF Agent]
        end
        subgraph "LLM Layer"
            LC[LLM Config]
            AC[Agent Config]
            PROV[LLM Providers]
        end
        subgraph "Agents"
            HA[Health Agent]
            FA[Future Agents...]
        end
        subgraph "Session Management"
            SM[Session Manager]
            CACHE[Cache System]
        end
    end

    %% Infrastructure Connections
    FRONT --> COOL
    COOL --> CFT
    FRONT --> CFW
    CFT --> API
    CFW --> API

    %% Flux de données
    API --> AA
    FC --> DA
    FT --> REA
    CPF --> CPFA
    
    AA --> INDM
    DA --> INDM
    REA --> INDM
    CPFA --> INDM
    
    DA --> RE
    REA --> RE
    CPFA --> RE
    
    INDM --> ME
    ME --> RNCP
    ME --> TRENDS
    ME --> REMP
    ME --> CPFI
    
    RNCP --> SF
    TRENDS --> SF
    REMP --> LSA
    CPFI --> LSA
    
    SF --> CA
    CA --> RG
    LSA --> SO
    
    LC --> HA
    AC --> HA
    
    RE --> SF
    RG --> CM
    CM --> RE

    %% Nouveaux flux
    SO --> SA
    SO --> RA
    SO --> RF
    SA --> SF
    HA --> SO
    HA --> SM
    SM --> CACHE
    LC --> PROV
    PROV --> HA
    PDF --> SM
    
    %% User Document RAG Flow
    FRONT --> SUP
    SUP --> UD
    API --> DPA
    DPA --> UD
    DPA --> DC
    DPA --> DPS
    UD --> DC
    DC --> HA
    DC --> CA
    HA --> |User-specific RAG| DC

    %% Styles
    classDef primary fill:#2374ab,stroke:#2374ab,color:#fff
    classDef secondary fill:#ff7e67,stroke:#ff7e67,color:#fff
    classDef storage fill:#57a773,stroke:#57a773,color:#fff
    classDef agent fill:#7d5ba6,stroke:#7d5ba6,color:#fff
    classDef llm fill:#ffa07a,stroke:#ffa07a,color:#fff
    classDef userRag fill:#9370DB,stroke:#9370DB,color:#fff
    
    class FC,FT,CPF secondary
    class ME,RE,SUP storage
    class HA,FA,LSA agent
    class DA,AA,REA,CPFA,INDM,CM,DPA primary
    class LC,AC llm
    class UD,DC,DPS userRag
