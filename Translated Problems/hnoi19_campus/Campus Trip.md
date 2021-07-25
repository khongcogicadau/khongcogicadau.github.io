# Campus Trip

Mỗi tòa nhà trong trường của Nam được gán một số riêng biệt. Một ngày nọ Nam cảm thấy chán và quyết định đi dạo quanh khuôn viên trường.

Nam đã đi học tại trường một thời gian và rất quen thuộc với những con số của các tòa nhà, vì vậy Nam quyết định ghi lại những con số của những tòa nhà mình đi qua. Nhưng trên thực tế, Nam không thực sự ghi lại những con số đó mà là số dư của chúng cho $2$, hay gọi là nhãn của tòa nhà. Nhãn của các tòa nhà liên tiếp kết hợp với nhau tạo thành một chuỗi.

Nam rất hứng thú với những chuỗi này, đặc biệt khi chúng đối xứng, vì vậy Nam quyết định sẽ làm một cuộc khảo sát.

Trường của Nam có thể biểu diễn bởi một đồ thị vô hướng, trong đó các tòa nhà là các đỉnh và các hànhlang là các cạnh của đồ thị. Mỗi đỉnh sẽ có một nhãn là $0$ hoặc $1$. Nam sẽ chọn ra một số cặp đỉnh và muốn biết rằng liệu có tồn tại một đường đi giữa hai đỉnh này sao cho nhãn của các đỉnh trên đường đi tạo thành một chuỗi đối xứng. Bên cạnh đó, những đường đi không nhất thiết là đường đi đơn.

Cho biết các thông tin về đồ thị, hãy giúp Nam hoàn thành cuộc khảo sát.

## Input format

Dòng đầu tiên chứa ba số nguyên $N, M, Q$ lần lượt là số đỉnh, số cạnh của đồ thị và số câu hỏi của Nam.

Dòng thứ hai chứa một xâu nhị phân độ dài $N$, kí tự thứ $i$ là nhãn của đỉnh $i$.

$M$ dòng tiếp theo, mỗi dòng chứa hai số nguyên $u, v$ thể hiện có cạnh nối giữa $u$ và $v$. Đảm bảo rằng không có khuyên hay cạnh lặp trong đồ thị.

$Q$ dòng cuối cùng, mỗi dòng chứa hai số nguyên $x, y$ thể hiện một câu hỏi của Nam.

## Output format

In ra $Q$ dòng, mỗi dòng là $\texttt{YES}$ hoặc $\texttt{NO}$. In ra $\texttt{YES}$ nếu tồn tại một đường đi thỏa mãn và $\texttt{NO}$ trong trường hợp ngược lại.

## Sample

### Input

```
5 4 2
00010
4 5
1 3
4 2
2 5
3 5
1 3
```

### Output

```
NO
YES
```

### Input

```
10 11 10
0011011111
4 6
10 6
5 9
4 7
10 7
5 8
1 9
5 7
1 10
5 1
5 6
10 3
7 4
8 10
9 4
8 9
6 6
2 2
9 9
10 9
3 4
```

### Output

```
NO
YES
YES
NO
YES
YES
YES
YES
YES
NO
```

## Subtask

- $30\%$ số test có $M \le 10000$.

- $40\%$ số test khác có $N\le 1000$ và $M\le 50000$.

- Các test còn lại thỏa mãn $N\le 5000$; $M\le 500000$ và $Q\le 100000$.