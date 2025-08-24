# Guia de Comandos Git

Um resumo rápido dos principais comandos Git para consulta rápida.

---

## 📦 Configurando um Novo Projeto
| Comando | Descrição |
|---------|-----------|
| `git init` | Inicializa um novo repositório Git no diretório atual |
| `git remote add origin <url>` | Conecta o repositório local com um servidor remoto |
| `git commit -am "Primeiro commit"` | Prepara e faz commit de todos os arquivos rastreados com uma mensagem |
| `git push --origin main` | Envia a branch principal para o remoto e configura o rastreamento upstream |

---

## 🌿 Trabalhando com Branches
| Comando | Descrição |
|---------|-----------|
| `git branch -a` | Lista todas as branches, incluindo as remotas |
| `git checkout -b feature/nova-feature` | Cria e muda para uma nova branch |
| `git push -u origin feature/nova-feature` | Envia a nova branch para o remoto e configura rastreamento upstream |
| `git branch -d feature/nova-feature` | Deleta uma branch local após a fusão |

---

## ✏️ Lidando com Mudanças
| Comando | Descrição |
|---------|-----------|
| `git add -p` | Adiciona mudanças interativamente, permitindo a seleção de partes específicas |
| `git commit --amend` | Modifica o último commit, permitindo atualizar a mensagem ou adicionar novas alterações |
| `git reset --hard HEAD~2` | Desfaz os últimos dois commits, descartando mudanças localmente |
| `git stash push -m "Trabalho em progresso"` | Salva mudanças atuais com uma descrição personalizada |

---

## 🤝 Colaboração
| Comando | Descrição |
|---------|-----------|
| `git fetch origin` | Busca mudanças do remoto sem mesclar |
| `git merge origin/main` | Mescla mudanças da branch principal remota na branch atual |
| `git rebase -i HEAD~3` | Rebases interativamente os três últimos commits para um histórico limpo |
| `git cherry-pick <commit-hash>` | Aplica um commit específico de outra branch |

---

## 📜 Histórico e Rastreamento
| Comando | Descrição |
|---------|-----------|
| `git log --oneline --graph --decorate --all` | Mostra o histórico de commits em gráfico visual compacto |
| `git diff HEAD^ HEAD` | Mostra as mudanças introduzidas pelo último commit |
| `git blame <arquivo> -L 10,20` | Mostra quem alterou as linhas de 10 a 20 de um arquivo |

---

## 🏷️ Gerenciando Tags
| Comando | Descrição |
|---------|-----------|
| `git tag -a v1.0 -m "Versão 1.0 Liberada"` | Cria uma tag anotada para uma versão com mensagem |
| `git push origin v1.0` | Envia a tag para o repositório remoto |

---

## 🌐 Lidando com Remotos
| Comando | Descrição |
|---------|-----------|
| `git remote -v` | Lista todos os repositórios remotos configurados com seus URLs |
| `git fetch --all --prune` | Busca mudanças de todos os remotos e remove branches remotas obsoletas |

---

## 🔄 Desfazendo Mudanças
| Comando | Descrição |
|---------|-----------|
| `git reset --soft HEAD^` | Desfaz o último commit mas mantém as mudanças preparadas para re-commit |
| `git checkout -- <arquivo>` | Descarta mudanças locais em um arquivo, revertendo para o último commit |

---

> 💡 Dica: Você pode manter este README aberto no VSCode ou no navegador para consulta rápida durante o dia a dia.
