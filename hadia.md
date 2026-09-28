# step 1 next.js folder
first we open window then type cmd after cmd open we type cd desktop then nxp create-next-app@latest my name 
hadia.nextjs
cd hadia.nextjs
npm install@supbase/supabase.js
npm run dev

# step 2
supabase + stores and manage database data. Connection Next.js connects to supabase using 
You can add, read, update, and delet and from supabase in your Next.js app.
Example: login system, products, users, notes, or orders.

# step 3
import { createClient } from '@supabase/
supabase-js'

const supabase = createClient 
 'YOUR_SUPABASE_URL',

YOUR_SUPABASE_AWON_KEY'
)
export default supabase

# Step 4
import { createClient } from '@supabase/
supabase-js'

export const supabase = createClient(
    process.env.NEXT-PUBLIC-SUPABASE-URL,
    process.env.NEXT-PUBLIC-SUPABASE-ANON-KEY
)
import { supabase } from '../lib/supabase'

export default function Home() {
    return <h1>NEXT.js + Supabase Connected</h1>
}
