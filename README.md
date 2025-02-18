import pandas as pd
import ace_tools as tools

# Criando a tabela minuciosa de estudo
data = {
    "Dia": [
        "Segunda-feira", "Segunda-feira", "Segunda-feira", "Segunda-feira",
        "Terça-feira", "Terça-feira", "Terça-feira", "Terça-feira",
        "Quarta-feira", "Quarta-feira", "Quarta-feira", "Quarta-feira",
        "Quinta-feira", "Quinta-feira", "Quinta-feira", "Quinta-feira",
        "Sexta-feira", "Sexta-feira", "Sexta-feira", "Sexta-feira",
        "Sábado", "Sábado", "Sábado", "Sábado"
    ],
    "Horário": [
        "08:00 - 10:00", "10:00 - 12:00", "14:00 - 16:00", "16:00 - 18:00",
        "08:00 - 10:00", "10:00 - 12:00", "14:00 - 16:00", "16:00 - 18:00",
        "08:00 - 10:00", "10:00 - 12:00", "14:00 - 16:00", "16:00 - 18:00",
        "08:00 - 10:00", "10:00 - 12:00", "14:00 - 16:00", "16:00 - 18:00",
        "08:00 - 10:00", "10:00 - 12:00", "14:00 - 16:00", "16:00 - 18:00",
        "08:00 - 10:00", "10:00 - 12:00", "14:00 - 16:00", "16:00 - 18:00"
    ],
    "Disciplina": [
        "Direito Penal", "Direito Processual Penal", "Direito Penal", "Direito Processual Penal",
        "Direito Constitucional", "Direito Administrativo", "Direito Constitucional", "Direito Administrativo",
        "Direitos Humanos", "Legislação Penal Especial", "Direitos Humanos", "Legislação Penal Especial",
        "Criminologia", "Medicina Legal", "Criminologia", "Medicina Legal",
        "Disciplina Específica PF/GO/DF/MG", "Disciplina Específica PF/GO/DF/MG", "Disciplina Específica PF/GO/DF/MG", "Disciplina Específica PF/GO/DF/MG",
        "Revisão Semanal", "Resolução de Questões", "Revisão Semanal", "Resolução de Questões"
    ],
    "Assunto": [
        "Teoria do Crime", "Inquérito Policial", "Culpabilidade", "Provas no Processo Penal",
        "Princípios Constitucionais", "Poderes Administrativos", "Organização do Estado", "Responsabilidade Civil do Estado",
        "Tratados Internacionais de DH", "Lei de Drogas", "Convenções Internacionais", "Lei Maria da Penha",
        "Escolas Criminológicas", "Perícias Médico-Legais", "Teorias do Crime", "Autópsias e Exames Médicos",
        "Direito Civil (PF)", "Legislação Estadual (GO)", "Legislação Institucional (DF)", "Legislação Estadual (MG)",
        "Resumo de todos os tópicos estudados na semana", "Simulados com questões de concursos anteriores", "Esquemas e mapas mentais", "Casos práticos e questões discursivas"
    ],
    "Tópico/Subtópico": [
        "Conceito, Elementos, Tipicidade", "Fases, Abertura e Condução", "Erro de Tipo e Proibição", "Prova Ilícita e Exceções",
        "Fundamentos e Supremacia da Constituição", "Atributos e Características", "Organização Federativa", "Reparação de Danos",
        "Declarações Universais", "Tráfico de Drogas", "Direitos Humanos na ONU", "Medidas Protetivas",
        "Clássica, Positivista e Crítica", "Identificação de Indivíduos", "Fatores Sociais do Crime", "Necropsias e Diagnósticos",
        "Obrigações Contratuais (PF)", "Prerrogativas de Delegados (GO)", "Normas da PCDF", "Direitos do Servidor (MG)",
        "Revisão com Flashcards", "Treinamento com tempo cronometrado", "Análise de erros", "Correção comentada de provas discursivas"
    ],
    "Dicas de Estudo": [
        "Livro: Cleber Masson - Direito Penal", "Código de Processo Penal Comentado", "Curso do Renato Brasileiro", "Resolução de questões do Cebraspe",
        "Curso do Pedro Lenza", "Livro do Matheus Carvalho", "Constituição Federal Anotada", "Jurisprudência do STF/STJ",
        "Material do Estratégia Concursos", "Lei 11.343/06 - Comentada", "Declarações da ONU", "Artigos sobre violência doméstica",
        "Livro de Criminologia do Nilo Batista", "Manual de Medicina Legal", "Mapa mental das teorias criminológicas", "Aulas de peritos criminais",
        "Vade Mecum (Saraiva) para consulta", "Legislação Estadual disponível nos sites das PC's", "Material oficial da PCDF", "Resolução de simulados específicos",
        "Refaça resumos de pontos fracos", "Crie fichas de memorização", "Releia anotações da semana", "Treinamento de redação com limite de linhas"
    ]
}

# Criando DataFrame
df = pd.DataFrame(data)

# Exibir a tabela ao usuário
tools.display_dataframe_to_user(name="Plano de Estudos Detalhado para Delegado (PF, GO, DF, MG)", dataframe=df)
