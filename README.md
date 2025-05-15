fmt.Println(calculate(0.8, 0.4, 1.88))
}

func calculate (a float, b float, x float) float {
    numerator := math.Pow(math.Pow(x-a, 2), 1/8) + math.Pow(x+b, 1/5)

    fmt.Println(numerator)

    denominator := math.Pow(math.Pow(x, 3)-math.Pow(a+b, 2), 1/9)

    fmt.Println(denominator)

    result := numerator / denominator
    
    return result
}
} 
