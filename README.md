# FunAI2025
![Static Badge](https://img.shields.io/badge/Python-%3E%3D3.10.0-green)<br>
以下是我參加 FunAI Camp 2025 的資料。
將會隨著時間累積而增加。

## `MLGame`
Requirement: `python >= 3.10.0`
```
pip install -r requirements.txt
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu118
```

### `MLGame` > `arkanoid`
玩遊戲指令: `python -m mlgame -f 120 -i ./ml/ml_play_template.py . --level 5`<br>
手動玩遊戲指令: `python -m mlgame -f 120 -i ./ml/ml_play_manual.py . --level 5`<br>
蒐集遊戲指令+不顯示畫面: `python -m mlgame -f 120 --nd -i ./ml/play.py . --level 5`<br>
訓練遊戲（不需要用到 MLGgame 框架）:`python ml/model_train_classification.py `<br>
訓練後玩遊戲指令: `python -m mlgame -f 120 -i ./ml/model_play_classification.py . --level 5`

### `MLGame` > `racing_car`
玩遊戲指令: `python -m mlgame -f 120 -i ml/ml_play_template.py ./ --game_type NORMAL --car_num 40 --racetrack_length 10000  --round 5 --sound off`<br>
手動玩遊戲指令: `python -m mlgame -f 120 -i ml/ml_play_manual.py ./ --game_type NORMAL --car_num 40 --racetrack_length 10000  --round 5 --sound off`<br>
RL 訓練遊戲指令: `python -m mlgame -f 120 -i ml/rl_training_PPO.py ./ --game_type NORMAL --car_num 40 --racetrack_length 10000  --round 5 --sound off`<br>
RL 玩遊戲指令: `python -m mlgame -f 120 -i ml/rl_play_PPO.py ./ --game_type NORMAL --car_num 40 --racetrack_length 10000  --round 5 --sound off`<br>
訓練遊戲指令+不顯示畫面: `python -m mlgame -f 120 --nd -i ml/rl_training_PPO.py ./ --game_type NORMAL --car_num 40 --racetrack_length 10000  --round 5 --sound off` <br>

## `Notes`
Notes 是我所製作的筆記，會按時更新！😄