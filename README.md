# -Interpretaci-n-simb-lica
Derecho penal
import React from 'react';
import { useState } from 'react';

type Row = {
  Generación: string;
  Interpretación_simbólica: string;
  Tratamiento_del_código: string;
  Derecho_penal: string;
};

const App = () => {
  const initialData: Row[] = [
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: "Las genealogías no deben entenderse como simples listas de linaje, sino como códigos simbólicos que contienen orden espiritual; romper con ellas es alterar el significado sagrado del ser.",
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Transgresión de la conciencia generacional"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Violación del linaje espiritual"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Ruptura del pacto ancestral"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Negación del origen sagrado"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Desobediencia al orden simbólico"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Alteración de la identidad heredada"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Falsificación del símbolo de pertenencia"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Ocultamiento del legado espiritual"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Desvinculación de la historia interna"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Anulación de la herencia profética"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Perjuicio a la estructura del alma colectiva"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Inversión del símbolo sagrado"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Rechazo del código del linaje"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Fragmentación del archivo espiritual"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Profanación del orden interior"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Omisión del testimonio intergeneracional"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Destrucción del hilo simbólico"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Exilio del símbolo familiar"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Quebrantamiento del mandamiento onírico"
    },
    {
      Generación: "👨👩 → 👩",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Negligencia en la transmisión del código"
    },
    {
      Generación: "👨👩 → 👨",
      Interpretación_simbólica: '""',
      Tratamiento_del_código: "Código simbólico",
      Derecho_penal: "Silencio frente al linaje: delito de olvido"
    }
  ];

  const [data, setData] = useState<Row[]>(initialData);

  return (
    <div className="container mx-auto p-4">
      <h1 className="text-2xl font-bold mb-4 text-gray-800">Genealogical Table</h1>
      <div className="overflow-x-auto">
        <table className="min-w-full bg-white border border-gray-300 rounded-md shadow-md">
          <thead className="bg-gray-100">
            <tr>
              <th className="py-2 px-4 border-b text-left text-gray-700">Generación</th>
              <th className="py-2 px-4 border-b text-left text-gray-700">Interpretación Simbólica</th>
              <th className="py-2 px-4 border-b text-left text-gray-700">Tratamiento del Código</th>
              <th className="py-2 px-4 border-b text-left text-gray-700">Derecho Penal</th>
            </tr>
          </thead>
          <tbody>
            {data.map((row, index) => (
              <tr key={index} className={index % 2 === 0 ? "bg-gray-50" : ""}>
                <td className="py-2 px-4 border-b text-gray-700">{row.Generación}</td>
                <td className="py-2 px-4 border-b text-gray-700">{row.Interpretación_simbólica}</td>
                <td className="py-2 px-4 border-b text-gray-700">{row.Tratamiento_del_código}</td>
                <td className="py-2 px-4 border-b text-gray-700">{row.Derecho_penal}</td>
              </tr>
            ))}
          </tbody>
        </table>
      </div>
    </div>
  );
};

export default App;
