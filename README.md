
# Chess Move Prediction Model

This repository contains a program that uses neural networks to predict the next move in a chess game based on the current board state. The project demonstrates data preprocessing, model training, and inference using a chess dataset.

---

## Features
- Preprocess chess games in PGN/CSV format to extract board states and moves.
- Train a neural network to predict the next move.
- Visualize training progress (accuracy and loss plots).
- Use the trained model to infer the next move for any chessboard state (in FEN format).

---

## Requirements
- Python 3.7 or higher
- Required libraries:
  - `numpy`
  - `pandas`
  - `python-chess`
  - `tensorflow`
  - `scikit-learn`
  - `matplotlib`

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## Dataset
This program uses the `games.csv` dataset containing chess games in PGN format. You can replace this file with any other chess game dataset with similar structure.

---

## How to Fork and Run
1. **Fork the Repository**:
   - Click the "Fork" button at the top-right of this repository to copy it to your GitHub account.

2. **Clone the Repository**:
   - Run the following command in your terminal to clone the repository:
     ```bash
     git clone https://github.com/FestinBiju/chess-move-prediction.git
     cd chess-move-prediction
     ```

3. **Add the Dataset**:
   - Place your `games.csv` file in the project root directory.

4. **Install Dependencies**:
   - Ensure you have Python installed.
   - Run:
     ```bash
     pip install -r requirements.txt
     ```

5. **Run the Program**:
   - Open the Jupyter notebook:
     ```bash
     jupyter notebook Chess_Move_Prediction_Model.ipynb
     ```
   - Follow the instructions in the notebook to preprocess data, train the model, and make predictions.

---

## File Structure
- `Chess_Move_Prediction_Model.ipynb`: Jupyter Notebook containing the full implementation.
- `games.csv`: The dataset (must be added separately).
- `requirements.txt`: List of dependencies for the project.

---

## How to Use
1. **Preprocess Data**:
   - The notebook extracts board states and moves from the dataset.
2. **Train the Model**:
   - Train the neural network using the dataset.
3. **Make Predictions**:
   - Input a chessboard state in FEN format to predict the next move.

---

## Visualization
Training progress is visualized using Matplotlib, with plots for:
- Training and validation accuracy.
- Training and validation loss.

---

## Example Prediction
Use the function `predict_next_move(fen)` to predict the next move:
```python
test_fen = 'rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - 0 1'
predicted_move = predict_next_move(test_fen)
print(f"Predicted move: {predicted_move}")
```

---

## Contributing
Contributions are welcome! Please fork the repository, make your changes, and create a pull request.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
For questions or suggestions, feel free to contact me via [GitHub Issues](https://github.com/FestinBiju/chess-move-prediction/issues).
