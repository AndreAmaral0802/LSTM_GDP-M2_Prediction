# LSTM_GDP-M2_Prediction

Use the LSTM deep learning to predict GDP and Money Supply growth in percentage changes.

The project needs some adjustements on the parameters but it is almost done. 

Despite all adjustments the model suffers from the black swan effect, in other words, the model is not capables of capturing the drastic changes on the GDP 
due to the abrupt drop caused by the covid-19 crisis and the sharp rise that happened after the lockdown. 

The concept:
Long Short-Term Memory (LSTM) is a type of recurrent neural network (RNN) architecture that is particularly effective in handling sequence data and capturing long-term dependencies. Unlike traditional RNNs, LSTM networks address the vanishing gradient problem, which can occur when training models on long sequences, by incorporating memory cells and gating mechanisms.

The key concept behind LSTM is its ability to selectively remember and forget information over time, allowing it to retain relevant information while discarding irrelevant or redundant information. LSTM networks consist of memory cells, input gates, output gates, and forget gates, which collectively enable the network to manage and process sequential data efficiently.

The LSTM architecture involves the following components:

Memory cells: These are responsible for storing and updating the information over time. The cells are equipped with a cell state (also known as the long-term memory) that runs along the entire sequence.

Input gates: These gates regulate the flow of information into the memory cells. They determine which parts of the incoming data should be stored in the cell state.

Output gates: These gates control the flow of information out of the memory cells. They decide which parts of the cell state should be outputted at each time step.

Forget gates: These gates determine which information to discard from the cell state. They learn to forget unnecessary information and prevent it from influencing future predictions.

The LSTM network processes sequential data in a step-by-step manner:

Input processing: At each time step, the LSTM network receives an input and combines it with the previous output and cell state.

Gate operations: The input gate determines which parts of the input should be stored in the cell state. The forget gate decides which information from the previous cell state should be discarded. The output gate determines which parts of the cell state should be outputted.

Cell state update: The network updates the cell state by combining the input gate-selected information and the forget gate-filtered previous cell state.

Output generation: The network generates the output by passing the updated cell state through the output gate.

LSTM networks are widely used in various applications, such as natural language processing, speech recognition, time series analysis, and machine translation. Their ability to capture long-term dependencies makes them especially suitable for tasks where context and temporal information are crucial.

By incorporating memory cells and gating mechanisms, LSTM networks provide a powerful solution for effectively processing and modeling sequential data. Their ability to handle long-term dependencies makes them a valuable tool in understanding and predicting patterns in time series and sequential data.
