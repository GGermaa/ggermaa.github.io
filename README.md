import matplotlib.pyplot as plt
from matplotlib.widgets import TextBox

textoax = plt.axes([0.1, 0.5, 0.5, 0.1])
texto = TextBox(ax=textoax, initial="test", label="testing")
texto.on_text_change(lambda v: print(v))

plt.show()
