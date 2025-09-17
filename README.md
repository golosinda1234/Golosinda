

<!DOCTYPE html>
<html>
<head>
    <title>Chess Board</title>
</head>
<body>
    <h2>Create a script using nested for loop that creates a chess board.<br>
    Use table width="270px" and take 30px as cell height and width.<br>
    Use bgcolor #FFFFFF and #000000.</h2>

    <table width="270px" cellspacing="0" cellpadding="0" border="1">
        <?php
        for ($row = 1; $row <= 8; $row++) {
            echo "<tr>";
            for ($col = 1; $col <= 8; $col++) {
                // Alternate cell color
                $total = $row + $col;
                if ($total % 2 == 0) {
                    $color = "#FFFFFF"; // white
                } else {
                    $color = "#000000"; // black
                }
                echo "<td bgcolor='$color' height='30px' width='30px'></td>";
            }
            echo "</tr>";
        }
        ?>
    </table>
</body>
</html>
