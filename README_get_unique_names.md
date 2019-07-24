def gen_unique_names(names,surnames,how_many):
    answer = []
    while how_many > 0:
        combo = choice(names)+' '+choice(surnames)
        if combo not in answer:
            answer.append(combo)
            how_many -= 1
    return answer

mynamelist = gen_unique_names(names,surnames,20)
for item in mynamelist:
    print item
