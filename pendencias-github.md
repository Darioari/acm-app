# Pendências GitHub — Darioari (repo acm-automacao-juridica/mendes-cruz-app)
Levantado em 2026-10-07 a partir das notificações (8 itens).

## Abertas (precisam de ação sua)

### #221 — [Design · aprovação Dario] Painel de Administração de tenants
- Status: aberta. Você aprovou o design com 5 ajustes e entregou mockups (#252 painel, #251 planos e créditos).
- O Augusto abriu a #266 (fundação: is_platform_admin + ciclo de vida do tenant), commit adfcb32.
- Próximo passo seu: revisar a #266 e, depois que ela for mergeada, abrir o PR de produção (actions + UI) trocando os mocks por queries reais.

### #238 — Aviso: RBAC Fase C (PRs #226–#237) tocou áreas do Jullio e do Dario
- Status: aberta, você está atribuído (junto com o Jullio).
- Para você saber: toda server action de escrita precisa de `await assertPode("<modulo>","criar|editar|excluir")` logo após o requireAuth(). Ações novas de escrita devem incluir o gate.
- PR #239: RBAC híbrido do PARCEIRO. O escopo é o teto e a matriz do perfil restringe por dentro. `DEFAULT_PARCEIRO` em lib/auth/permissoes.ts é espelho do seed do banco: se mudar um, mude o outro.
- Pessoas (#232, #233) é área sua.
- O Jullio abriu o PR #291 (banner de erro do modal Novo lead). Aguarda validação e merge do Augusto.

## Fechadas / nada pendente
- #219 [Dario] Finalizar #210: fechada como não planejada. Pessoas já está em produção (#228/#229), a busca da Biblioteca já está no main, o shell #133 foi abandonado.
- #133 Shell 3 painéis de Petições: fechada definitivamente como não planejada (PO, 08/07). O mockup está defasado. Não reabrir.
- #210 PR: fechado sem merge.
- #128 Pessoas: fechada pela #228.
- #163 @floating-ui/dom: corrigida na #218 (mergeada).
- #99 Módulo Petições: fechada, já em produção.

## Resumo
Só 2 itens com ação real: #221 (revisar #266 e depois fazer o PR de UI real) e #238 (conhecer o padrão assertPode; o #291 do Jullio aguarda o Augusto).
