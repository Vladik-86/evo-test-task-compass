def direction(facing, turn):
    # your smart code here
    direction =  ['N', 'NE', 'E', 'SE', 'S', 'SW', 'W', 'NW']
    start_face = direction.index(facing)
    turns = (turn // 45) + start_face
    d_lens = len(direction)
    end_face = turns % d_lens
    return direction[end_face]