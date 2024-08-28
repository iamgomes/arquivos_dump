### Importando os models

from avaliacoes.models import Avaliacao
from usuarios.models import User
from questionarios.importa_questionarios import gera_avaliacao

a = Avaliacao.objects.get(pk=1)
u = User.objects.get(pk=1)
gera_avaliacao(u, a, 'MT')
