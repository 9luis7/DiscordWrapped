# 🚀 Features Futuras - Discord Wrapped

## 📋 Otimização 2: Consolidar Sessões Consecutivas

### **O que é:**
Lógica para agrupar sessões de voz consecutivas do mesmo usuário no mesmo canal.

### **Como funcionaria:**
- Verificar última sessão do usuário
- Se foi no mesmo canal e tempo entre fim/anterior < 3 minutos
- Consolidar em uma única sessão

### **Exemplo:**
```
ANTES:
- Sessão 1: 10:00-10:05 (5min)
- Sessão 2: 10:07-10:15 (8min)  ← 2min de diferença
- Sessão 3: 10:16-10:20 (4min)  ← 1min de diferença

DEPOIS:
- Sessão consolidada: 10:00-10:20 (20min total)
```

### **Benefícios:**
- ✅ Dados mais precisos
- ✅ Reflete intenção real do usuário
- ✅ Remove "ruído" de pausas curtas

### **Complexidade:**
- 🔴 Alta (lógica de agrupamento)
- 🔴 Risco de bugs
- 🔴 Testes complexos

### **Status:**
- 📝 Anotado para Versão 2.0
- ⏳ Aguardando implementação do sistema de relatórios
- 🎯 Prioridade: Média

---

## 📊 Outras Features Futuras

### **Análise com Pandas**
- Relatórios semanais/mensais
- Gráficos de atividade
- Estatísticas avançadas

### **Reset Automático Mensal**
- Cron job para resetar dados
- Backup antes do reset
- Notificação de reset

### **Comandos Avançados**
- Exportar dados
- Comparar períodos
- Rankings personalizados
