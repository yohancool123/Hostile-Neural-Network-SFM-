name "Hostile Neural Network"

every 20 ticks do
    input fe:: from "Power" top side
    output fe:: to "S1","S2","S3","S4","S5","S6","S7","S8","S9","S10","S11","S12","S13","S14","S15","S16"
end

every 20 ticks do
    input prediction_matrix from "Me Network"
    output 2 to each "S1","S2","S3","S4","S5","S6","S7","S8","S9","S10","S11","S12","S13","S14","S15","S16" ROUND ROBIN BY LABEL
    forget

    input from "S1","S2","S3","S4","S5","S6","S7","S8","S9","S10","S11","S12","S13","S14","S15","S16" slots 2
    output to "Me Network"
    forget

    input hostilenetworks:prediction from "S1"
    output to "F1"
    forget

    input hostilenetworks:prediction from "S2"
    output to "F2"
    forget

    input hostilenetworks:prediction from "S3"
    output to "F3"
    forget

    input hostilenetworks:prediction from "S4"
    output to "F4"
    forget

    input hostilenetworks:prediction from "S5"
    output to "F5"
    forget

    input hostilenetworks:prediction from "S6"
    output to "F6"
    forget

    input hostilenetworks:prediction from "S7"
    output to "F7"
    forget

    input hostilenetworks:prediction from "S8"
    output to "F8"
    forget

    input hostilenetworks:prediction from "S9"
    output to "F9"
    forget

    input hostilenetworks:prediction from "S10"
    output to "F10"
    forget

    input hostilenetworks:prediction from "S11"
    output to "F11"
    forget

    input hostilenetworks:prediction from "S12"
    output to "F12"
    forget

    input hostilenetworks:prediction from "S13"
    output to "F13"
    forget

    input hostilenetworks:prediction from "S14"
    output to "F14"
    forget

    input hostilenetworks:prediction from "S15"
    output to "F15"
    forget

    input hostilenetworks:prediction from "S16"
    output to "F16"
    forget
end
