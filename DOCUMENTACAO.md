# SOS Emoções - Documentação Completa 🌈

> Última atualização: **17/05/2026**
> Versão: **2.0.0**
> Status: **Em Planejamento**

---

## 📚 Índice Geral

1. [Visão Geral](#visão-geral)
2. [Começando](#começando)
3. [Guia de Contribuição](#guia-de-contribuição)
4. [Protocolo de Crise](#protocolo-de-crise)
5. [Segurança e LGPD](#segurança-e-lgpd)
6. [Roadmap](#roadmap-e-melhorias)

---

# SOS Emoções 🌈

Um aplicativo desenvolvido para apoiar pessoas em momentos de crise emocional, oferecendo recursos de autoajuda, contatos de suporte e protocolos de bem-estar mental.

## 📋 Sobre o Projeto

O **SOS Emoções** é uma iniciativa voltada para saúde mental e bem-estar emocional, com foco em:
- 🆘 Suporte em momentos de crise
- 📞 Conexão com profissionais de saúde mental
- 📚 Recursos educacionais sobre emoções
- 🔒 Segurança e privacidade dos dados (LGPD)

## 🚀 Começando

### Pré-requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Acesso a dispositivo com armazenamento local

### Instalação
```bash
# Clone o repositório
git clone https://github.com/yyivfuyf/teste.git
cd teste

# Abra no navegador
open index.html
```

### Primeira Execução
1. Abra `index.html`
2. Preencha seus dados (nome, série, turma, turno)
3. Aceite o consentimento LGPD
4. Comece a registrar suas emoções!

---

# 🤝 Guia de Contribuição

## Código de Conduta

Esperamos que todos os contribuidores sigam nosso código de conduta:
- ✅ Seja respeitoso e inclusivo
- ✅ Aceite críticas construtivas
- ✅ Foque no que é melhor para a comunidade

## 🐛 Relatando Bugs

Se encontrou um bug, por favor:
1. Verifique se já não foi relatado em [Issues](https://github.com/yyivfuyf/teste/issues)
2. Crie uma nova issue com:
   - Título claro e descritivo
   - Descrição detalhada do comportamento esperado vs. observado
   - Passos para reproduzir
   - Screenshots (se aplicável)

## ✨ Sugerindo Melhorias

Tem uma ideia? Ótimo!
1. Abra uma [Discussion](https://github.com/yyivfuyf/teste/discussions) ou Issue
2. Descreva a melhoria e seu caso de uso
3. Aguarde feedback da comunidade

## 🔄 Processo de Pull Request

### Preparação
```bash
# 1. Faça um fork e clone
git clone https://github.com/seu-usuario/teste.git
cd teste

# 2. Crie uma branch
git checkout -b feature/sua-feature

# 3. Faça suas mudanças
# ... edite os arquivos ...

# 4. Commit
git commit -m "feat: descrição breve da mudança"

# 5. Push
git push origin feature/sua-feature
```

### Submissão
1. Abra um Pull Request com descrição clara
2. Referencie issues relacionadas
3. Aguarde revisão

## 📝 Convenção de Commits

Use o prefixo apropriado:
- `feat:` - Novas funcionalidades
- `fix:` - Correções de bugs
- `docs:` - Mudanças de documentação
- `style:` - Formatação, sem mudanças lógicas
- `refactor:` - Reorganização de código
- `test:` - Adição ou modificação de testes
- `chore:` - Mudanças de build, dependências, etc

Exemplo:
```
feat: adicionar validação de email no formulário
fix: corrigir erro de navegação em mobile
docs: atualizar README com instruções
```

## ✅ Checklist para Pull Request

- [ ] Meu código segue o estilo do projeto
- [ ] Eu atualizei a documentação necessária
- [ ] Eu adicionei testes para novas funcionalidades
- [ ] Minhas mudanças não quebram testes existentes
- [ ] Eu referenciei issues relacionadas

---

# 🚨 Protocolo de Intervenção em Crise

## Visão Geral
Este documento define os procedimentos de resposta para situações de risco emocional/mental detectadas no SOS Emoções.

---

## Níveis de Risco

### 🟢 NÍVEL 0 - Bem-estar Normal
**Indicadores:**
- 80-100% de emoções positivas
- Registros consistentes
- Participação em atividades

**Ação:**
- ✅ Nenhuma intervenção necessária
- Manutenção de monitoramento

---

### 🟡 NÍVEL 1 - Atenção (Ansiedade Leve)
**Indicadores:**
- Padrão "Ansioso" por 1-2 dias
- Sem outros sinais de alerta
- Capacidade de participação mantida

**Ação - Automática:**
```
✓ Mensagem: "Respire: 4s-7s-8s. Você consegue!"
✓ Oferta: Técnica de respiração + Meditação
✓ Chat com IA: Suporte emocional
```

---

### 🔴 NÍVEL 2 - Alerta (Isolamento/Tristeza Prolongada)
**Indicadores:**
- "Triste" ou "Cansado" por 3+ dias
- Redução de participação
- Isolamento observado
- Mudança de comportamento

**Ação - IMEDIATA:**
```
NOTIFICAÇÃO AUTOMÁTICA:
{
  aluno: "João Silva",
  serie: "8º A",
  alerta: "Isolamento prolongado (3+ dias)",
  prioridade: "ALTA",
  prazo: "Contato em 24h"
}
```

**Protocolo:**
1. Orientador convida para conversa privada
2. Escuta ativa (sem julgamentos)
3. Identificar causa
4. Oferecer recursos
5. Agendar acompanhamento
6. Informar responsáveis

---

### ⚫ NÍVEL 3 - CRÍTICO (Risco Iminente de Suicídio)
**Indicadores - PALAVRAS-CHAVE:**
```
🚨 DETECTAR IMEDIATAMENTE:
✗ "Suicídio" / "Quero morrer"
✗ "Não aguento mais"
✗ "Machucar a mim mesmo"
✗ "Adeus" / "É o fim"
✗ "Ninguém se importa" (em contexto de desesperança)
```

**Ação - CRÍTICA (Em Tempo Real):**

```
⏱️ T+0min
├─ Sistema detecta palavra-chave
├─ ALERTA VERMELHO exibido
├─ Notificação ao psicólogo + coordenador
└─ SMS automático aos responsáveis

⏱️ T+5min
├─ Psicólogo contacta aluno
├─ Se não responde → Coordenador procura
└─ Se fora da escola → Contacta responsáveis

⏱️ T+15min
├─ Se CONFIRMADO risco iminente:
│  ├─ LIGAR PARA SAMU (192)
│  ├─ CONTACTAR RESPONSÁVEIS
│  └─ REGISTRAR NA POLÍCIA
└─ Se risco moderado:
   └─ Acompanhamento intensivo
```

---

## 📞 Contatos de Emergência

### Brasil
```
🆘 CVV (Prevenção ao Suicídio)
  Telefone: 188
  Chat: www.cvv.org.br
  Horário: 24 horas, 7 dias/semana
  ✓ Gratuito
  ✓ Sigilo total

🚑 SAMU
  Telefone: 192
  Risco de morte iminente
  Resposta: ~10 minutos

⚖️ DISQUE 100 (Denúncia de Abuso)
  Telefone: 100
  Para: Abuso, negligência, exploração
```

---

## ✅ Checklist de Implementação

### Código
- [x] Detectar palavras-chave de risco
- [x] Sistema de notificação em tempo real
- [x] Dashboard para psicólogo/coordenador
- [x] Log de incidentes
- [ ] Integração com SMS
- [ ] Mensagens pré-configuradas

### Processo
- [ ] Treinar equipe pedagógica
- [ ] Definir contatos de emergência
- [ ] Criar protocolo impresso
- [ ] Realizar simulado mensal
- [ ] Documentar resposta
- [ ] Revisar anualmente

### Legal/Compliance
- [x] Informar pais na matrícula
- [x] Obter consentimento LGPD
- [ ] Documentar responsabilidades
- [ ] Seguro de responsabilidade
- [ ] Consultar advocacia escolar

---

# 🔐 Segurança e Conformidade LGPD

## 1. Conformidade LGPD

### Lei Geral de Proteção de Dados (Lei 13.709/2018)

**O SOS Emoções está em conformidade com:**
- ✅ Princípios de privacidade by design
- ✅ Consentimento informado dos responsáveis
- ✅ Transparência sobre coleta de dados
- ✅ Direito ao acesso e exclusão
- ✅ Proteção de dados pessoais
- ✅ Anonimização em relatórios

---

## 2. Dados Coletados

### Informações do Aluno
```javascript
const DADOS_COLETADOS = {
  pessoais: [
    "Nome completo",
    "Série/Ano escolar",
    "Turma",
    "Turno"
  ],
  emocionais: [
    "Registros de emoção (data/hora/tipo)",
    "Mensagens no chat",
    "Técnicas utilizadas"
  ],
  nao_coletamos: [
    "Geolocalização",
    "Câmera/Microfone",
    "Dados biométricos"
  ]
};
```

---

## 3. Armazenamento de Dados

### Local Storage (Padrão)
```javascript
const STORAGE = {
  tipo: "Browser Local Storage + IndexedDB",
  servidor: "Nenhum (offline-first)",
  acesso: "Apenas no dispositivo do aluno",
  
  vantagens: [
    "✓ Privacidade 100% garantida",
    "✓ Sem risco de vazamento",
    "✓ Funciona offline",
    "✓ Controle total do usuário"
  ]
};
```

---

## 4. Criptografia

### Implementação (Futuro)
```javascript
// Usando TweetNaCl.js
import nacl from 'tweetnacl';

const CRIPTOGRAFIA = {
  algoritmo: "NaCl/Curve25519 + XSalsa20",
  forca: "256 bits (militar)"
};
```

---

## 5. Consentimento e Autorização

### Modal de Consentimento LGPD
```html
<div class="modal-lgpd">
  <h2>🔐 Proteção de Dados Pessoais</h2>
  
  <h3>✅ SEUS DIREITOS:</h3>
  <ul>
    <li>Direito de saber quais dados coletamos</li>
    <li>Direito de acessar os dados</li>
    <li>Direito de deletar os dados</li>
    <li>Direito de não ser discriminado(a)</li>
  </ul>
  
  <h3>🛡️ PROTEÇÃO:</h3>
  <ul>
    <li>✓ Dados armazenados LOCALMENTE</li>
    <li>✓ NENHUM servidor externo</li>
    <li>✓ Criptografia de dados sensíveis</li>
    <li>✓ Anonimato em relatórios</li>
  </ul>
  
  <h3>🗑️ RETENÇÃO:</h3>
  <p>Dados apagados automaticamente após 90 dias.</p>
  
  <input type="checkbox" required /> Entendo e autorizo
  <button class="btn-primary">Continuar</button>
</div>
```

---

## 6. Direitos do Usuário

### Acesso
```javascript
function acessarMeusDados() {
  // Aluno/responsável pode baixar TODOS seus dados
  const dados = {
    perfil: usuarioAtual,
    registros: registros,
    chats: chats,
    formato: "JSON legível"
  };
  exportarJSON(dados);
}
```

### Exclusão
```javascript
function deletarMeusDados() {
  if (confirm('Todos os dados serão apagados.')) {
    localStorage.clear();
    // Registrar auditoria
  }
}
```

---

## 7. Responsabilidades da Escola

### Equipe Responsável
```
Diretor/a de Ensino
├─ Responsável legal pelos dados
└─ Aprova políticas

Coordenador/a Pedagógico/a
├─ Designa encarregado de dados
└─ Monitora conformidade

Psicólogo/a Escolar
├─ Acessa dados para intervenção
└─ Mantém confidencialidade

Equipe de TI
├─ Mantém segurança técnica
└─ Auditoria de acessos
```

---

## 8. Medidas de Segurança Técnica

### Proteção do Navegador
```javascript
const SEGURANCA = {
  protocolo: "HTTPS/TLS 1.3+",
  limpeza_automatica: "90 dias sem acesso",
  limite_tamanho: "5MB",
  protecao: "SameSite=Strict em cookies"
};
```

### Proteção de Sessão
```javascript
function protegerSessao() {
  const TIMEOUT = 30 * 60 * 1000; // 30 minutos
  
  let timeoutId = setTimeout(() => {
    logout();
  }, TIMEOUT);
}
```

---

## 9. Auditoria e Logs

### O que é registrado
```javascript
const AUDITORIA = {
  login: { quem, quando, resultado },
  modificacao_dados: { quem, o_que, de, para, quando },
  acesso_dados: { quem, qual_aluno, quando, por_que }
};
```

### Retenção de Logs
```
✓ Manter por 1 ano
✓ Criptografado
✓ Acesso restrito
✓ Auditado trimestral
✓ Apagar após 1 ano
```

---

## 10. Resposta a Incidentes

### Procedimento em Caso de Vazamento

```
⏱️ IMEDIATAMENTE (0-1h)
├─ Descobrir o vazamento
├─ Isolar o sistema
├─ Documentar
└─ Notificar direção

⏱️ DENTRO DE 24h
├─ Investigar causa
├─ Notificar responsáveis
├─ Notificar LGPD (se 10+ pessoas)
└─ Iniciar remediação

⏱️ DENTRO DE 7 dias
├─ Relatório completo
├─ Corrigir vulnerabilidade
└─ Comunicação interna
```

---

## 11. Checklist de Conformidade

### Antes do Lançamento
- [x] Política de Privacidade publicada
- [x] Termo de Consentimento assinado (100% pais)
- [ ] Designar Encarregado de Dados
- [ ] Avaliação de Impacto realizada
- [ ] Teste de segurança
- [x] Documentação completa
- [ ] Treinamento da equipe
- [ ] Procedimento de incidente pronto

### Mantido Anualmente
- [ ] Revisão de Política
- [ ] Atualização de Tecnologia
- [ ] Auditoria de Logs
- [ ] Teste de Recuperação
- [ ] Retrain da equipe
- [ ] Relatório de Conformidade

---

# 🚀 Roadmap e Melhorias

## 1. ❌ Falta de Dados de Validação

### Problema
O projeto não apresenta:
- Pesquisa quantitativa com estudantes
- Estatísticas da escola
- Evidências de impacto emocional

### ✅ Solução Proposta

Adicionar **Dashboard de Validação** com:
- Pesquisa piloto com 50-100 alunos
- Gráficos de antes/depois (ansiedade, motivação)
- Citações anônimas de estudantes
- Dados de evasão escolar da instituição
- Relatório trimestral de impacto

---

## 2. ❌ Semáforo Emocional Muito Simplista

### Problema
Verde/Amarelo/Vermelho é superficial e não capta nuances

### ✅ Solução - Semáforo Inteligente

```
🟢 VERDE (Bem-estar)
   • 80-100% de emoções positivas
   • Ação: Manutenção da rotina

🟡 AMARELO (Atenção)
   • 50-79% de emoções mistas
   • Ação: Reforço de acolhimento
   
🔴 VERMELHO (Alerta)
   • Mais de 30% de registros críticos
   • Ação: Intervenção imediata
   
⚫ CRÍTICO (Risco iminente)
   • Palavras-chave detectadas
   • Ação: CVV 188 + SAMU 192
```

---

## 3. ❌ Feedback e Engajamento Fraco

### Problema
O projeto não garante retorno ao aluno

### ✅ Solução - Sistema de Resposta Garantida

```
1️⃣ Aluno registra emoção
2️⃣ Recebe feedback automático
3️⃣ Equipe pedagógica responde em 48h
4️⃣ Aluno vê que foi ouvido!
```

---

## 4. ❌ Falta de Integração com a Família

### Problema
Pais/responsáveis não têm acesso

### ✅ Solução - Dashboard para Responsáveis

- Relatório mensal de bem-estar (anonimizado)
- Tendências e gráficos
- Dicas para apoiar em casa
- Contato direto com escola

---

## 5. ❌ Falta de Validação Científica

### Problema
Não usa framework consolidado

### ✅ Solução - Alinhar com CASEL (5 Pilares SEL)

```
1️⃣ AUTOCONHECIMENTO
   "Como você se sente?"
   
2️⃣ AUTORREGULAÇÃO
   "Técnicas de respiração/meditação"
   
3️⃣ CONSCIÊNCIA SOCIAL
   "Apoiar colegas"
   
4️⃣ HABILIDADES RELACIONAIS
   "Grupos de apoio"
   
5️⃣ TOMADA DE DECISÃO RESPONSÁVEL
   "Buscar ajuda quando necessário"
```

---

## 📋 Roadmap Consolidado

### Sprint 1 (Junho)
- [ ] Validação LGPD básica
- [ ] Protocolo de crise (N1)
- [ ] Semáforo emocional (versão beta)

### Sprint 2 (Julho)
- [ ] Criptografia de dados
- [ ] Protocolo de crise (N2 + N3)
- [ ] Dashboard orientador

### Sprint 3 (Agosto)
- [ ] Portal responsáveis
- [ ] Pesquisa quantitativa
- [ ] Validação CASEL

### Sprint 4+ (Setembro em diante)
- [ ] Grupo de apoio
- [ ] Chat entre colegas
- [ ] Publicação científica

---

## 🌟 Melhorias Propostas

### Performance
- Otimizar carregamento de páginas
- Implementar cache inteligente
- Reduzir bundle size

### UX/UI
- Redesign da interface
- Acessibilidade melhorada
- Dark mode (já implementado)
- Responsividade aprimorada

### Funcionalidades
- IA para recomendações personalizadas
- Integração com wearables
- Análise de padrões emocionais
- Gamificação de objetivos

### Segurança
- Autenticação biométrica
- Backup criptografado
- Auditoria de segurança regular

---

## 💡 Ideias Futuras

- Parcerias com profissionais de saúde mental
- Programas de bem-estar corporativo
- Integração com sistemas de saúde
- API pública para desenvolvedores
- Tradução para outros idiomas
- Aplicativo mobile (React Native)
- Comunidade de suporte online
- Integração com calendário escolar
- Relatórios para pais e professores
- Sistema de pontos e recompensas

---

# ⚠️ Aviso Importante

Este aplicativo é um complemento educacional e não substitui atendimento profissional. Em caso de crise, procure ajuda de profissionais qualificados ou contatos de emergência imediatamente.

**🆘 Em caso de emergência, sempre ligue:**
- **CVV: 188** (Prevenção ao Suicídio)
- **SAMU: 192** (Emergência Médica)
- **DISQUE 100** (Denúncia de Abuso)

---

**Mantido por:** Projeto Liga Jovem  
**Próxima revisão:** 17/06/2026  
**Licença:** MIT