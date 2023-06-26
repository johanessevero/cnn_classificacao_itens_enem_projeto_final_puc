# CLASSIFICAÇÃO DE ITENS DO EXAME NACIONAL DO ENSINO MÉDIO (ENEM)

<p>O presente trabalho se propõe a explorar a utilização de um modelo de machine learning para classificar um item elaborado para o Exame Nacional do Ensino Médio com base no texto do item e no texto das alternativas, dentro de quatro faixas de valores do parâmetro de discriminação, parâmetro de dificuldade e o parâmetro de acerto ao acaso, ou seja, pretende-se resolver um problema de classificação de texto. Esse problema se situa no processo de aprendizagem supervisionada, no campo da Inteligência Artificial. Isso pode ajudar no processo de uma avaliação educacional, como o Enem, porque permite uma seleção mais eficiente e precisa de itens para a avaliação. Essa classificação com base nas faixas de valores dos parâmetros de dificuldade, discriminação e acerto ao acaso pode permitir a identificação de itens que possuem características desejáveis, tais como uma boa discriminação entre os participantes que dominam e não dominam a habilidade avaliada, e uma dificuldade apropriada para a avaliação. O uso de um modelo de classificação de itens pode ser uma ferramenta valiosa para melhorar a qualidade e a eficiência da avaliação educacional.</p>
<p>O modelo de classificação de itens do Enem pode fornecer uma estimativa inicial dos parâmetros de discriminação, dificuldade e acerto ao acaso, porém, não eliminando a necessidade de realização de um pré-teste para validar a precisão desses valores. Isso porque existem muitos fatores que podem afetar o desempenho dos itens, como a clareza e a concisão da pergunta, o nível de habilidade dos participantes, entre outros. Portanto, o pré-teste permitiria ajustar e validar esses valores antes de utilizá-los para fins de avaliação.</p>

Após avaliação do modelo concluiu-se que houve overffiting no treinamento e o conjunto de dados disponíveis não é suficientemente grande e representativo, é preciso obter mais dados de treinamento e isso não é viável no momento para o projeto em questão. Mas, apesar de o desempenho da rede neural convolucional ter sido ruim houve a oportunidade de se passar por todos os passos de treinamento e avaliação de um modelo. Eventualmente se houver mais dados o modelo pode ser utilizada como base.

Os dados de texto dos itens coletados foram inseridos no dataset "df_itens_geral.csv" com os seguintes campos:

- co_posicao: Indica a posição do item no conjunto de questões.
- sg_area: Representa a área à qual o item pertence.
- co_item: Código identificador do item.
- tx_gabarito: Contém a letra correspondente à resposta correta do item.
- co_habilidade: Código que identifica a habilidade associada ao item.
- in_item_aban: Indica se o item foi abandonado ou não.
- tx_motivo_aban: Descreve o motivo pelo qual o item foi abandonado, caso aplicável.
- nu_param_a, nu_param_b, nu_param_c: Parâmetros da TRI associados ao item.
- tx_cor: Cor da prova em que o item foi aplicado.
- co_prova: Código que identifica a prova em que o item foi aplicado.
- id: Identificador único do item.
- ano: Ano em que o item foi aplicado.
- cor: Cor da prova em que o item foi aplicado.
- meio_aplicacao: Meio de aplicação do item (ex: papel).
- num_questao: Número da questão.
- area: Área à qual a questão pertence.
- texto_questao: Texto da questão.
- texto_base: Texto base para a resolução da questão.
- alternativa_a, alternativa_b, alternativa_c, alternativa_d, alternativa_e: Alternativas de resposta disponíveis para a questão.
- tp_lingua: Tipo de língua em que a questão foi redigida.
- in_item_adaptado: Indica se o item foi adaptado ou não.
- tp_versao_digital: Tipo de versão digital do item.
