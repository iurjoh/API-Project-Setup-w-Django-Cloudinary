# Exercício de configuração Django e Cloudinary

**Português (Brasil)** | [English](README.md)

Exercício inicial de configuração Django com armazenamento de mídia Cloudinary. O nome cita configuração de API, mas as URLs revisadas têm apenas administração Django; não é apresentado como API concluída.

**Documentação revisada:** 01/10/2026. Nenhum teste, migração ou execução foi feito.

## Objetivo e registro de desenvolvimento

Começa do template de aluno da Code Institute. Há `manage.py` e configurações/URLs em `API_PROJECT/`. O README anterior era orientação genérica de template, não planejamento do projeto. Não inventamos processo de design ou histórico de funcionalidades concluídas.

## Arquitetura e configuração

O projeto Django fica em `API_PROJECT/`. `urls.py` inclui apenas `admin/`. As configurações usam SQLite (`db.sqlite3`) e classe de mídia Cloudinary.

A configuração está incompleta: entradas adjacentes de `INSTALLED_APPS` não têm vírgulas, concatenando strings em nomes inválidos de apps. Nenhum `requirements.txt` foi encontrado na raiz; esta revisão não permite reproduzir a instalação por uma lista fixada de dependências.

## Segurança antes de reutilizar

O arquivo público tem `SECRET_KEY` de desenvolvimento literal e `DEBUG` ligado. Não reutilize essa chave em serviço publicado. Use chave nova gerenciada por ambiente em qualquer instalação real e reveja debug, hosts, credenciais de mídia e acesso. Esta documentação não reproduz ou usa a chave, altera configurações ou publica o app.

## Status de configuração local

Não trate as instruções antigas do template como receita validada. Primeiro corrija `INSTALLED_APPS`, registre dependências, separe segredos locais e valide a configuração. Depois, use ambiente isolado e dados fictícios para `python3 manage.py check` antes de migração ou execução. Nenhuma execução bem-sucedida é afirmada aqui.

## Design, testes e snapshots

É configuração de backend, não interface finalizada. A revisão leu configurações, URLs, `manage.py` e README anterior. Checagens futuras devem cobrir configuração, migrações, mídia e permissões. Screenshots datados de exemplos seguros devem ficar em `docs/assets/`; nenhum snapshot novo foi embutido.

## Créditos e licença

Template de aluno Code Institute e software de terceiros Django/Cloudinary. Nenhum `LICENSE` foi encontrado na raiz. Preserve seus termos; esta atualização não aplica MIT a código de terceiros nem trata notas de versão do template como histórico do autor.
