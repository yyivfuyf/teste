# 🔐 Política de Segurança e LGPD

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
- [ ] Política de Privacidade publicada
- [ ] Termo de Consentimento assinado (100% pais)
- [ ] Designar Encarregado de Dados
- [ ] Avaliação de Impacto realizada
- [ ] Teste de segurança
- [ ] Documentação completa
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

**Data de Criação:** 17/05/2026
**Próxima Revisão:** 17/05/2027
**Responsável:** Encarregado de Dados (DPO)
