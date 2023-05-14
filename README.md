def get_action(current_state, reward_matrix):
    available_action = []
    print("reward_matrix","\n",reward_matrix)    
    for action in enumerate(reward_matrix[current_state]):     
        if action[1]!= -1:            
            available_action.append(action[0]) 
    choose_action = random.choice(available_action)
    print("Random choice of action from",available_action,"is", choose_action)           
    return choose_action
