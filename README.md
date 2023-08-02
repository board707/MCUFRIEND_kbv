MCUFRIEND_kbv port for W80x controllers
===========

This is a version of MCUFRIEND_kbv library with a support of w80x controllers. I will make a pull request to original MCUFRIEND_kbv repository.

## Connections

<table>
    <thead>
        <tr>
            <th>LCD pins</th>
            <th>W80x pins, var 1 </th>
            <th>W80x pins, var 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="center">LCD_D0</td>
            <td align="center">PB0</td>
            <td align="center">PB4</td>
        </tr>
        <tr>
            <td align="center">LCD_D1</td>
            <td align="center">PB1</td>
            <td align="center">PB5</td>
        </tr>
        <tr>
            <td align="center">LCD_D2</td>
            <td align="center">PB2</td>
            <td align="center">PB6</td>
        </tr>
        <tr>
            <td align="center">LCD_D3</td>
            <td align="center">PB3</td>
            <td align="center">PB7</td>
        </tr>
        <tr>
            <td align="center">LCD_D4</td>
            <td align="center">PB4</td>
            <td align="center">PB8</td>
        </tr>
        <tr>
            <td align="center">LCD_D5</td>
            <td align="center">PB5</td>
            <td align="center">PB9</td>
        </tr>
        <tr>
            <td align="center">LCD_D6</td>
            <td align="center">PB6</td>
            <td align="center">PB10</td>
        </tr>
        <tr>
            <td align="center">LCD_D7</td>
            <td align="center">PB7</td>
            <td align="center">PB11</td>
        </tr>
        <tr>
            <td align="center">LCD_RD</td>
            <td colspan =2 align="center">PA7</td>
        </tr>
        <tr>
            <td align="center">LCD_WR</td>
            <td colspan =2 align="center">PA8</td>
        </tr>
        <tr>
            <td align="center">LCD_RS</td>
            <td colspan =2 align="center">PA9</td>
        </tr>
        <tr>
            <td align="center">LCD_CS</td>
            <td colspan =2 align="center">PA10</td>
        </tr>
        <tr>
            <td align="center">LCD_RST</td>
            <td colspan =2 align="center">PA11</td>
        </tr>
    </tbody>
</table>

Pinout variant 2 mostly uses pins that don't have alternative features like PWM or SPI. However, the display output may be slightly slower in this case.
To choose between options, uncomment one of the lines **`#define USE_W80X_PINOUT1`** or **`#define USE_W80X_PINOUT2`** at the beginning of the file `utility/mcufriend_special.h`.

## Links
[FastLED library](https://github.com/FastLED/FastLED)

[W80x Arduino package](https://github.com/board707/w80x_arduino)

Original MCUFRIEND_kbv [README](README_orig.md).
