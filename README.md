# Robots
В классе GameWindow:
- занес m_visualizer в метод, так как он нигде не переиспользуется

В классе LogWindow:
- сделал m_logSource и m_visualizer константами

В классе GameVisualizer:
- занес m_timer в метод GameVisualizer
- в методе Timer вместо создания переменной timer теперь возвращается сразу new Timer
- в методе onModelUpdateEvent удалил переменную velocity
- в методе moveRobot удалил переменную newDirection
- метод applyLimits, переписал вот так - return value > min && value < max ? value : value < min ? min : max;
